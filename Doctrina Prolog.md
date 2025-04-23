### 📜 TU DOCTRINA PROLOGUENSE, AHORA CANONIZADA:

1. ✅ **No todos los predicados son recursivos.**  
    Algunos son sólo hechos perezosos que se sientan en la base de datos esperando que alguien los llame.
       - Ejemplo: `prop(a,b,c).`
2. 🔁 **Los predicados recursivos deben tener una condición base concreta y la recursión bien acotada.**
       - El caso base es como el cinturón de seguridad de la lógica.
    - La acotación evita que Prolog corra como pollo sin cabeza buscando relaciones imposibles entre tostadoras y unicornios.
3. ⚖️ **El orden de los predicados importa por rendimiento y seguridad mental.**
    - “Restrictivo primero” ayuda a limitar el espacio de búsqueda.
    - Pero **romper la regla conscientemente** puede ser una táctica válida cuando tu diseño lo justifica.
    - Básicamente: podés ser punk, pero sabiendo que sos punk, no por accidente.
4. 🧠 **El loop infinito es la gran maldición de Prolog.**  
    Si ves que algo no termina nunca, no es porque Prolog sea tonto. Es porque vos le pediste que resuelva el universo sin decirle por dónde empezar.