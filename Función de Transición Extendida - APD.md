Con el objeto de implementar un analizador sintáctico Bottom-Up, vamos a extender la definición de la [[Función de Transición - APD|función de transición]] $\delta$ (APD extendido).  
Originalmente teníamos,  $$\delta : Q \times (\Sigma \cup \{\lambda\}) \times \Gamma \to 2^{Q \times \Gamma^*}  $$Ahora,  $$\delta : Q \times (\Sigma \cup \{\lambda\}) \times \Gamma^* \to 2^{Q \times \Gamma^*}$$
