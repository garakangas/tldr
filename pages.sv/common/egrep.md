# egrep

> Hitta mönster i filer med hjälp av utökade regexes.
> Obs: Det här kommandot är ett alias för `grep --extended-regexp`.
> Mer information: <https://manned.org/egrep>.

- Sök efter ett eller flera upprepade tecken:

`egrep '{{a}}+' {{sökväg/till/fil}}`

- Sök efter noll eller en förekomst av ett tecken (valfri träff):

`egrep '{{a}}?' {{sökväg/till/fil}}`

- Sök efter 10 repetitioner av ett tecken:

`egrep '{{a}}{10}' {{sökväg/till/fil}}`

- Sök efter 3 till 7 repetitioner av ett tecken:

`egrep '{{a}}{3,7}' {{sökväg/till/fil}}`

- Sök efter ett av de angivna alternativen:

`egrep '{{katt}}|{{hund}}|{{mus}}' {{sökväg/till/fil}}`

- Sök efter ett av de angivna alternativen som del av ett större mönster:

`egrep 'k({{a}}|{{i}}|{{o}})l' {{sökväg/till/fil}}`

- Sök efter en grupp av tecken som upprepas en eller flera gånger:

`egrep '({{aeiou}})+' {{sökväg/till/fil}}`

- Sök med hjälp av standardiserade teckenklasser (mer information: <https://www.regular-expressions.info/posixbrackets.html>):

`egrep [[{{:alnum:|:alpha:|:space:|...}}]] {{sökväg/till/fil}}`
