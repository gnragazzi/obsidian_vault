#### Definición

- Supongamos que $i_1,i_2,...,i_m$ es una [[Solución PCP|solución]] a una instancia de PCP.
- Consideremos las derivaciones de $G_{AB}$ 
$S\Rightarrow w_{i_1}Aa_{i_1}\Rightarrow w_{i_1}w_{i_2}Aa_{i_2}a_{i_1}\Rightarrow ... \Rightarrow w_{i_1}w_{i_2}...w_{i_{m-1}}Aa_{i_{m-1}}...a_{i_2}a_{i_1}\Rightarrow w_{i_1}w_{i_2}...w_{i_{m-1}}w_{i_{m}}a_{i_{m}}a_{i_{m-1}}...a_{i_2}a_{i_1}$
$S\Rightarrow x_{i_1}Ba_{i_1}\Rightarrow x_{i_1}x_{i_2}Ba_{i_2}a_{i_1}\Rightarrow ... \Rightarrow x_{i_1}x_{i_2}...x_{i_{m-1}}Ba_{i_{m-1}}...a_{i_2}a_{i_1}\Rightarrow x_{i_1}x_{i_2}...x_{i_{m-1}}w_{i_{m}}a_{i_{m}}a_{i_{m-1}}...a_{i_2}a_{i_1}$
- Cómo sabemos que $i_1,i_2,...,i_m$ es una solución, sabemos que $$w_{i_1}w_{i_2}...w_{i_m}=x_{i_1}x_{i_2}...x_{i_m}$$
- Por lo tanto, estamos derivando desde el símbolo distinguido hacia la misma cadena, siguiendo 2 derivaciones distintas. Por lo tanto, $G_{AB}$ es una [[Ambigüedad en GLC|GLC ambigüa]].

***
#### Etiquetas
- #falta 