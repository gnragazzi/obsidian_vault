|           |                                                                                                                          |
| --------- | ------------------------------------------------------------------------------------------------------------------------ |
| (repetir) | ... en toda la linea                                                                                                     |
| G         | desde la linea actual, hasta la última                                                                                   |
| $         | desde el caracter actual hasta el final de la linea                                                                      |
| 0         | desde el caracter anterior al cursor hasta el comienzo de la linea                                                       |
| l         | un caracter a la derecha                                                                                                 |
| f{c}      | hasta el próximo caracter {c} en la misma linea, incluyendo el caracter                                                  |
| F{c}      | hasta el anterior caracter{c} en la misma linea, incluyendo el caracter                                                  |
| t{c}      | hasta el próximo caracter {c} en la misma linea, sin incluir el caracter                                                 |
| T{c}      | hasta el anterior caracter {c} en la misma linea, sin incluir el caracter                                                |
| ;         | repite la última búsqueda de linea en la misma dirección                                                                 |
| ,         | repite la última búsqueda de linea en la dirección contraria                                                             |
| \{pat}    | hasta la próxima ocurrencia de {pat} en el documento                                                                     |
| ?{pat}    | hasta la anterior ocurrencia de {pat} en el documento                                                                    |
| n         | repite la última búsqueda de documento en la misma dirección                                                             |
| N         | repite la última búsqueda de documento en la dirección contraria                                                         |
| *         | hasta la próxima ocurrencia de la palabra bajo el cursor (incluyendo la palabra).                                        |
| w         | hasta el primer caracter de la próxima palabra                                                                           |
| aw        | la palabra entera bajo el cursor, incluido el espacio                                                                    |
| ap        | el parrafo entero al que pertenece la linea en la que está el cursor                                                     |
| gj,gk     | Mueve una display line hacia abajo/arriba                                                                                |
| W         | hasta el primer caracter de la próxima PALABRA                                                                           |
| b         | hasta la primer letra de la palabra actual (o la anterior si ya nos encontramos en la primer letra de la palabra actual) |
| B         | hasta la primer letra de la PALABRA actual (o la anterior si ya nos encontramos en la primer letra de la PALABRA actual) |
| e         | hasta el último caracter de la palabra actual (o la siguiente si...)                                                     |
| e         | hasta el último caracter de la PALABRA actual (o la siguiente si...)                                                     |
| ge        | hasta el último caracter de la palabra anterior                                                                          |
| gE        | hasta el último caracter de la PALABRA anterior                                                                          |
| i<t-o>    | selecciona todo lo que está entre el text object <t-o> \| POr lo general funciona mejor con c -> ci<t-o>                 |
| a<t-o>    | selecciona todo lo que está entre el <t-o>, <t-o> incluido \| Por lo general, funciona mejor con d -> da<t-o>            |