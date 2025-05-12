Características
-  Ambiente totalmente observable.  
- 2-jugadores.  
- suma cero.  
- determinísticos.  
- movimientos alternados.
***
Definición Formal
- Estado Inicial:
	- Configuración inicial del tablero
	- Información sobre quién mueve primero
- Función $jugador$ que dado un estado $s$, retorna a qué jugador le toca mover
- Función $acciones$ que dado un estado $s$ retorna el conjunto de acciones que son *legales* en dicho estado.
- La función sucesor (modelo de transición)
	- Dado un estado y una acción devuelve el estado resultante
- Test de estado $terminal: S\mapsto \{V,F\}$ 
	- Determina que estado es termnal
	- $T$ es el conjunto de estados terminales
- Función de utilidad $\mu:T\mapsto \mathbb{R}$  ^5d7fcc
	- Asigna un valor de utilidad a cada estado terminal desde el punto de vista de MAX
***
[[Árbol de Juego]] 
[[Estrategia Minimax]] 