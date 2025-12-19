####  **Demostración:** 
Por contradicción, supongamos que Le​ es decidible (recursivo). 
Entonces existe una MT **decididora** $R$ tal que, para cualquier entrada $⟨M⟩$, $R$ se detiene y acepta si $L(M)\ne∅$ y rechaza si $L(M)= ∅.$ 

Construimos una nueva MT decididora $S$ para el lenguaje universal $L_U$​ (que sabemos indecidible). $S$ recibe la entrada $⟨M,x⟩$ y opera así:

1. **Construcción:** $S$ construye la descripción de una nueva máquina $M′$ que, ante cualquier entrada $w$:
    - Ignora w.
    - **Simula** la ejecución de M sobre la entrada x.
    - **Si** la simulación de M sobre x entra en un estado de aceptación, entonces M′ acepta w.
    - _(Nota implícita: Si M rechaza o entra en bucle, M′ hace lo mismo y nunca acepta w)_.
2. **Consulta:** S ejecuta a R con la entrada ⟨M′⟩.
3. **Decisión:**
    - Si $R$ acepta (dice "No es Vacío"): Significa que $M′$ acepta alguna cadena (de hecho, las acepta todas). Esto implica que $M$ aceptó $x$. Entonces, $S$ **acepta** $⟨M,x⟩$.
    - Si R rechaza (dice "Es Vacío"): Significa que $M′$ no acepta ninguna cadena $w$. Esto implica que $M$ nunca aceptó $x$. Entonces, $S$ **rechaza** $⟨M,x⟩$.        

**Conclusión:** S decidiría $L_U$​, lo cual es imposible. La suposición inicial es falsa. $L_ne$​ no es decidible.
***
#### Etiquetas
- #Anki 