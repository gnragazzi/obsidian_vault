Sean $P$ y $Q$ [[Fórmula Lógica|fórmulas]] y $v$ una [[Función de Valuación]]. Entonces se tienen las siguientes propiedades/reglas
- $(R_\neg) v \text{ satisface a } \neg\neg P \leftrightarrow v \text{ satisface a }P$; $$R_\neg\qquad \frac{\neg\neg P}{P}$$   

- $(R_\lor) v \text{ satisface a } (P\lor Q) \leftrightarrow v \text{ satisface a }P \text{ o v satisface a }Q$$$R_\lor\qquad \frac{(P\lor Q)}{P|Q}$$
- $(R_{\neg\lor}) v \text{ satisface a } \neg(P\lor Q) \leftrightarrow v \text{ satisface a }\neg P \text{ y v satisface a }\neg Q$$$R_{\neg\lor}\qquad \frac{\neg(P\lor Q)}{\neg P,\neg Q}$$
- $(R_{\land}) v \text{ satisface a } (P\land Q) \leftrightarrow v \text{ satisface a }P \text{ y v satisface a }Q$ $$R_\land\qquad \frac{(P\land Q)}{P,Q}$$
- $(R_{\neg\land}) v \text{ satisface a } \neg(P\land Q) \leftrightarrow v \text{ satisface a }\neg P \text{ o v satisface a }\neg Q$ $$R_{\neg\land}\qquad \frac{\neg(P\land Q)}{\neg P|\neg Q}$$
- $(R_{\rightarrow}) v \text{ satisface a } (P\rightarrow Q) \leftrightarrow v \text{ satisface a }\neg P \text{ o v satisface a }Q$ $$R_\rightarrow\qquad \frac{(P\rightarrow Q)}{\neg P|Q}$$
- $(R_{\neg\rightarrow}) v \text{ satisface a } \neg(P\rightarrow Q) \leftrightarrow v \text{ satisface a }P \text{ y v satisface a }\neg Q$ $$R_{\neg\rightarrow}\qquad \frac{\neg(P\rightarrow Q)}{ P,\neg Q}$$
***
La forma de estas reglas es $$\frac{\text{premisa}}{\text{conclusión/conclusiones}}$$
Si  la premisa es [[Valuación que Satisface a una Fórmula|satisfacible]], alguna (o ambas) de sus conclusiones también lo es.
***
- En todos los casos se tiene que las conclusiones son o bien subfo ́rmulas o bien negaciones  de subfo ́rmulas de la correspondiente premisa.
- Se aplica la siguiente clasificación
	- Reglas de tipo A
		- Una valuación satisface a las premisas si y solo si satisface todas las conclusiones
	- Reglas de tipo B
		- Una valuación satisface la premisa si y solo si satisface al menos una de las conclusiones
	- 