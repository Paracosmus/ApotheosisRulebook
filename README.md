# Apotheosis Rulebook

Livro de regras do Apotheosis, publicado em [apotheosiscardgame.com](https://apotheosiscardgame.com). O site é gerado pelo [Retype](https://retype.com) a partir dos arquivos `.md` deste repositório.

## 1. Instalar

1. Instale o [Node.js](https://nodejs.org) (versão LTS).
2. Instale o Retype:

   ```powershell
   npm install retypeapp --global
   ```

3. Clone o repositório:

   ```powershell
   git clone git@github.com:Paracosmus/ApotheosisRulebook.git
   ```

## 2. Configurar a senha

As páginas com `visibility: protected` (como o Decklex) exigem uma senha. No site publicado, ela vem do secret `RETYPE_PASSWORD` do GitHub. Para rodar localmente, crie a mesma variável no seu sistema:

```powershell
[Environment]::SetEnvironmentVariable('RETYPE_PASSWORD', 'a-senha', 'User')
```

Feche e reabra o terminal (ou o VS Code inteiro) para a variável valer. Sem ela, o Retype mostra `No "password" project-level option is configured` e não gera essas páginas.

## 3. Rodar

Na pasta do repositório:

```powershell
retype start
```

O site abre em http://localhost:5001 e recarrega sozinho a cada arquivo salvo. `Ctrl+C` encerra.

## 4. Publicar

Faça push para a branch `main`. O GitHub Actions gera o site e o publica na branch `retype`, que o GitHub Pages serve.

Na primeira configuração do repositório:

1. Em **Settings → Secrets and variables → Actions**, crie os secrets `RETYPE_KEY` (chave do Retype Pro) e `RETYPE_PASSWORD`.
2. Em **Settings → Pages**, escolha a branch `retype` como origem.
