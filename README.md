# lita
```
<programa> ::= ISA AMPIDIRINA: \d+
               BAIKO: <baiko>
               ISA AVOAKA: <rafitrisa>

<baiko> ::= [F|f]oana. # Ny mot-clés afaka apetraka aorinan'ny teboka
                       # dia afaka atomboka amin'ny renin-tsoratra
          | raiso <voambolana> kasoloy <rafitrisa>.
          | raha <vina> dia <baiko> ratszay <baiko>.
          | ataovy <baiko> rambola <vina>.
          | tapaho.
          | `` <baiko> ''
          | <baiko>. <baiko>

<voambolana> ::= [a-z]+(\d|[a-z]|_)*

<rafitrisa> ::= -?\d+
              | fidirana[\d+]
              | <voambolana>
              | ( <rafitrisa> )
              | <rafitrisa> + <rafitrisa>
              | <rafitrisa> * <rafitrisa>
              | <rafitrisa> - <rafitrisa>
              | <rafitrisa> / <rafitrisa>

<vina> ::= marina
         | diso
         | <rafitrisa> <  <rafitrisa>
         | <rafitrisa> =  <rafitrisa>
         | ( <vina> )
         | <vina> na <vina>
         | <vina> sy <vina>
```
