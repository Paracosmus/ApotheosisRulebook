<!-- Insert this at the top of each markdown page -->

<!-- Global Functions -->
{{ p(value) = '<span class="positive">' + value + '</span>' }}
{{ n(value) = '<span class="negative">' + value + '</span>' }}
{{ req(condition) = '<span class="req">【</span> ' + condition + ' <span class="req">】</span>' }}


<!-- Message -->
{{

    review() = `
!!!danger
Esta seção ainda não foi completamente revisada. Algumas informações podem estar desatualizadas ou incompletas, e a formatação pode não estar finalizada.
!!!
    `

}}


<!-- Briefing -->
{{

    briefing(loc, brief) = `
|||{.briefing} [!badge text="` + loc + `" variant="ghost"]
  ` + brief + `
|||
    `

}}
