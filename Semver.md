Versionado Semántico
donde `<mayor>.<minor>.<patch>` 
- Major: dígito utilizado para indicar cambios mayores. Por ejemplo, cambios de firma, tecnología, etc.
- minor: para indicar cambios menores. Por ejemplo una nueva funcionalidad.
- patch: para indicar cambios rápidos y pequeños. Por ejemplo un hot-fix
***
A su vez, existen Flavors de las versiones, los cuales, al usar gitflow, son inferidos automáticamente.
- Si el **head branch** del pull request es **release/*:** El algoritmo aumentará en 1 el dígito de **minor**. También se especifica el tipo **-rc** como parte del nombre del versionado. A su vez, posee un número incremental, el cual aumenta en 1 por cada build que se cree para el mismo release base. X.(minor ↑1).X-rc-(incremental ↑1). Ejemplo: 1.0.0-rc-1
- Si el **head branch** del pull request es **hotfix/*:** El algoritmo aumentará en 1 el dígito de **patch**. También se especifica el tipo **-hotfix** como parte del nombre del versionado. A su vez, posee un número incremental, el cual aumenta en 1 por cada build que se cree para el mismo release base. X.X.(patch ↑1)-hotfix-(incremental ↑1). Ejemplo: 1.0.1-hotfix-1
- El **head branch** del pull request es un branch no releaseable: El algoritmo aumentará en 1 el dígito de **patch**. También se especifica el tipo **-test** como parte del nombre del versionado. A su vez, posee un número incremental, el cual aumenta en 1 por cada build que se cree para el mismo release base. X.X.(patch ↑1)-test-(incremental ↑1). Ejemplo: 2.0.1-test-1