1. [[Dot Command]] 
	1. [[x - Normal Mode]]
	2. [[d - Normal Mode]]
	3. [[> - Normal Mode]]
2. Don't Repeat Yourself
	1. [[Cambio (letra c)]] (C, S, s, o, O)
	2. [[Insert - Append]]
3. Take one step back, 3 steps forwards
4. Act, Repeat, Reverse
	1. [[Tabla de comandos de Repetición - Deshacer]]
5. Find and Replace by Hand
	1. [[Replace %s]]
	2. [[* operand]] 
6. Meet the dot formula
	1. One keystroke to place the cursor
	2. One Keystroke for an operation
7. Pause with your brush up
8. Chunk your Undo's
	1. Aprovechar la característica del comando deshacer (u), saliendo del [[Insert Mode]] después de cada cambio significativo.
9. Compose Repeatable Changes
	1. *Vim is optimized for repetition*. 
		1. Para aprovechar esto, hay que componer acciones repetibles.
		2. Esta es una buena métrica para saber cuál de las muchas maneras que tiene VIM de hacer las cosas conviene elegir.
	2. [[Motions|{aw}]] 
10. Use Counts to Do Simple Arithmetic
	1. [[ctrl a]]
	2. [[ctrl x]]
11. Don’t Count If You Can Repeat
	1. Sobre el uso de counts en operaciones del [[Normal Mode]] de tipo
		`<operators><count><motion>`
	2. Sobre la conveniencia de usarlo vs repetir (usando dot command)
12. Combine and Conquer (07/03/25)
	1. Presentación del concepto de [[Operators - VIM]] 
	2. [[gU - gu]]
	3. [[Diferencia entre t{c} y f{c} como motion]]
	4. [[Motions]] 
	5. [[gc]]  
13. Make Corrections Instantly from [[Insert Mode]] (07/03/2025)
	1. `<C-h>` borra un caracter en IM
	2. `<C-w>` borra una palabra en IM
	3. `<C-u>` borra desde el comienzo de la linea en IM
14. Get back to Normal Mode (07/03/2025)
	1. `<C-o>` entra en el modo *Insert-Normal*
15. Paste from a Register Without Leaving Insert Mode (08/03/2025)
	1. [[<c-r>]]`<c-r> + 0` permite pegar en [[Insert Mode]] el contenido del registro 0.
	2. 
16. Do Back-of-the-Envelope Calculations in Place (09/03/2025)
	1. [[<c-r>#^86bc33|Calculos en ExMode]]
17. Insert Unusual Characters by Character Code (10/03/2025)
	1. [[<c-v>]]. 
18. Insert Unusual Characters by Digraph (11/03/2025)
19. Overwrite Existing Text with Replace Mode (08/03/2025)
	1. [[R - Vim|R]]
20. Grok Visual Mode (08/03/2025)
	1. Se pueden utilizar patrones de búsqueda para seleccionar, utilizando el visual mode
	2. 
