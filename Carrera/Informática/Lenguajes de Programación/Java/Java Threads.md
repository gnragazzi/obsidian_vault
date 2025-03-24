El sistema multithread en Java depende de la clase `Thread`, sus métodos y la [[Interfaz - OOP|interfaz]] [[Runnable - Interfaz Java|`Runnable`]]. Todos los programas de Java se ejecutan a partir de un thread principal, llamado *main*.
***
- `public static Thread currentThread()` es un método que devuelve el thread actual.
- `<thread>.toString()` imprime su nombre, prioridad y grupo
***
Estados de un Thread en Java
- Running
- Bloqued
- Ready
- Suspended
- Terminated
***
Los threads tienen asociada una prioridad que, en caso de empate, determina el uso de CPU.
***
[[Threads]]