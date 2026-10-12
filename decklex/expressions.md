---
label: Expressões
icon: code
order: 100
---

# Expressões

Uma expressão é uma conta escrita como texto dentro de um `Expr`. Ela pode calcular um número, comparar valores ou combinar condições, e o resultado fica disponível na variável `$Expr`.

```json
{ "Expr": "($base + 2) * 3 > 10 && !$bloqueado" }
```

O resultado de uma expressão é sempre um número inteiro, um booleano ou um texto.

---

## Valores

| Tipo               | Como escrever                                        | {.compact}
| ---                | ---                                                  |
| Número inteiro     | `3`, `-9`, `0x1F`                                    |
| Número fracionário | `0.5`, `.35`, `3.`, `2e3`                            |
| Booleano           | `true`, `false`                                      |
| Texto              | `"abc"`, com `\"` para aspas e `\\` para barra       |
| Variável           | `$nome`                                              |

Uma variável é sempre escrita com `$` na frente do nome. Uma variável que ainda não recebeu valor vale `0`.

---

## Operadores

- **Aritmética:** `+` `-` `*` `/` `%` `^`
- **Sinal:** `-x`
- **Comparação:** `==` `!=` `<` `>` `<=` `>=`
- **Lógica:** `&&` (e), `||` (ou), `!` (não)
- **Texto:** `+` junta dois textos
- **Agrupamento:** `( )`, com quantos níveis forem necessários
- **Comentário:** `/* … */` e `// …`, ignorados no cálculo

A comparação funciona entre números e entre textos. A lógica só aceita booleanos.

### Ordem de cálculo

Sem parênteses, os operadores são calculados nesta ordem, do primeiro ao último:

1. `^`
1. `-x` e `!`
1. `*` `/` `%`
1. `+` `-`
1. `==` `!=` `<` `>` `<=` `>=`
1. `&&`
1. `||`

---

## Funções

Uma função é escrita com seus valores entre parênteses, separados por vírgula: `min($base, 3)`.

### Uso geral

| Função                 | O que devolve                                           | {.compact}
| ---                    | ---                                                     |
| `if(condição, a, b)`   | `a` se a condição for verdadeira, `b` se for falsa      |
| `min(a, b, …)`         | O menor dos valores                                     |
| `max(a, b, …)`         | O maior dos valores                                     |
| `floor(x)`             | `x` arredondado para baixo                              |
| `ceil(x)`              | `x` arredondado para cima                               |
| `round(x)`             | `x` arredondado para o inteiro mais próximo             |
| `math::abs(x)`         | `x` sem o sinal                                         |
| `typeof(x)`            | O tipo de `x`: `"int"`, `"float"`, `"boolean"`, `"string"`, `"tuple"` ou `"empty"` |

### Texto

| Função                           | O que devolve                              | {.compact}
| ---                              | ---                                        |
| `len(t)`                         | A quantidade de caracteres de `t`          |
| `str::to_lowercase(t)`           | `t` em minúsculas                          |
| `str::to_uppercase(t)`           | `t` em maiúsculas                          |
| `str::trim(t)`                   | `t` sem os espaços do início e do fim      |
| `str::from(x)`                   | `x` escrito como texto                     |
| `str::substring(t, início, fim)` | O trecho de `t` entre as duas posições     |

### Conjuntos

Um conjunto é uma lista de valores entre parênteses, como `(1, 2, 3)`. Ele só serve como valor de entrada de uma função.

| Função                         | O que devolve                                               | {.compact}
| ---                            | ---                                                         |
| `contains((1, 2, 3), x)`       | Verdadeiro se `x` estiver no conjunto                       |
| `contains_any((1, 2), (2, 9))` | Verdadeiro se algum valor do segundo estiver no primeiro    |
| `len((1, 2))`                  | A quantidade de valores do conjunto                         |

### Matemática

Todas levam o prefixo `math::`.

| Categoria                 | Funções                                                        | {.compact}
| ---                       | ---                                                            |
| Potência e raiz           | `pow(a, b)`, `sqrt(x)`, `cbrt(x)`, `hypot(a, b)`               |
| Logaritmo e exponencial   | `ln(x)`, `log(x, base)`, `log2(x)`, `log10(x)`, `exp(x)`, `exp2(x)` |
| Trigonometria             | `sin`, `cos`, `tan`, `asin`, `acos`, `atan`, `atan2(a, b)`     |
| Trigonometria hiperbólica | `sinh`, `cosh`, `tanh`, `asinh`, `acosh`, `atanh`              |
| Checagem de número        | `is_nan(x)`, `is_finite(x)`, `is_infinite(x)`, `is_normal(x)`  |

### Bits

| Função         | O que devolve                              | {.compact}
| ---            | ---                                        |
| `bitand(a, b)` | E bit a bit                                |
| `bitor(a, b)`  | Ou bit a bit                               |
| `bitxor(a, b)` | Ou exclusivo bit a bit                     |
| `bitnot(a)`    | Inversão dos bits                          |
| `shl(a, n)`    | `a` deslocado `n` bits para a esquerda     |
| `shr(a, n)`    | `a` deslocado `n` bits para a direita      |

---

## Arredondamento

O jogo não usa frações, como definem as [Diretrizes](/guidelines.md). Quando o resultado final de uma expressão é fracionário, ele é arredondado para baixo: `7 / 2.0` resulta em `3`.

A divisão entre dois números inteiros já resulta em um inteiro: `7 / 2` é `3`.

---

## Cuidados

!!!warning
Uma expressão que não pode ser calculada resulta em `false`, sem nenhum aviso. Isso vale para erro de escrita, divisão por zero, função que não existe e valor do tipo errado.
!!!

- **Inteiro e fracionário não são iguais no `==`.** `1 == 1.0` é falso. Como `^`, `floor`, `ceil`, `round`, `math::pow` e `math::sqrt` devolvem um número fracionário, `2 ^ 2 == 4` também é falso. Escreva `2 ^ 2 == 4.0`, ou use `<`, `>`, `<=` e `>=`, que comparam os dois tipos normalmente.
- **Todos os lados são calculados.** `&&`, `||` e `if` calculam todas as suas partes antes de decidir. `$x != 0 && 10 / $x > 1` falha quando `$x` é `0`, em vez de resultar em falso pela primeira parte.
- **Comparações não se encadeiam.** `1 < 2 < 3` falha. Escreva `1 < 2 && 2 < 3`.
- **Booleano não é número.** `true && 1` e `1 + true` falham.
- **Divisão de inteiro negativo arredonda em direção ao zero.** `-7 / 2` é `-3`, e `-7 % 3` é `-1`.
- **Uma expressão não altera variáveis.** `=`, `+=` e os demais operadores de atribuição falham.
- **Não há sorteio.** Não existe função de número aleatório.
