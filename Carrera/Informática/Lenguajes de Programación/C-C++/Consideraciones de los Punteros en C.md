```
Si X tiene un valor numérico
 - &x -> la dirección de memoria donde se guarda el valor numérico de x
 - x -> el valor numérico almacenado
 - *x -> el valor que se encuentra en la dirección de memoria x.
```
- ¿Cómo trabajar con arreglos (punteros) pasados como argumentos de funciones?:
```
int *a = (int *) malloc(sizeof(int)*L); // DECLARACIÓN DEL ARREGLO

void sumar1(int *a, int len);// PROTOTIPO DE LA FUNCIÓN
sumar1(a,L); // INVOCACIÓN A LA FUNCIÓN - ESTA FUNCIÓN MODIFICARÁ EL ARREGLO ORIGINAL
```
- ¿Cómo trabajar con arreglos bi-dimensionales pasados como argumentos de funciones?:
	- Queremos un arreglo `a[L][K]` 
	- ERROR
		```
		int **a = (int **) malloc(sizeof(int)*L*K); // declaración
		```
		- Pensá que lo que queremos declarar es un puntero (a) que contiene ***la dirección de memoria donde encontraremos L punteros*** a arreglos de enteros, de longitud K.
		- Es decir, que hay que pedir memoria para a, y para cada uno de los L punteros a arreglos de A
	- Posibilidad 1
		```
			void sumar2dim(int **a, int len1, int len2);// función 
			...
			int **a = (int **) malloc(sizeof(int *)*L);
		    for(int i = 0; i < L; i++)
			    a[i] = (int *) malloc(sizeof(int)*K); 
			sumar2dim(a,L,K);
		```
		- En este caso, declaramos el puntero a L arreglos de `int *`, y cada uno de los L arreglos a K enteros.
		- En este caso, las modificaciones dentro de la función se reflejan en el exterior.
	- Posibilidad 2
		- ¿Qué pasa cuando queremos que la asignación de memoria ocurra dentro de la función?
		```
		void colocar_memoria_y_sumar2dim(int **a, int len1, int len2)
		{
		    int **temp = (int **) malloc(sizeof(int *)*L);
		    for(int i = 0; i < L; i++)    
				temp[i] = (int *) malloc(sizeof(int)*K); 
			for(int i = 0; i < len1; i++)
	        ... // se realiza la suma
			a = temp;
		}
		...
		int arr**;
		colocar_memoria_y_sumar2dim(arr,L,K);
		```
		- Tras ejecutarse la función, el puntero `arr` seguirá apuntando a `0x0`... 
		- ¿Por qué? Porque al pasar el puntero como argumento se utiliza, y los cambios no se ven reflejados en el exterior. Para que el código funcione como esperamos, ***necesitamos la dirección donde se encuentra el espacio de memoria que apunta a un arreglo de L int \****
		- Para ello, debemos cambiar el encabezado de la función, agregar un operador de dirección y de desreferenciación a la invocación y la función
```
		void colocar_memoria_y_sumar2dim(int ***a, int len1, int len2)//un * más
		{
		    int **temp = (int **) malloc(sizeof(int *)*L);
		    for(int i = 0; i < L; i++)    
				temp[i] = (int *) malloc(sizeof(int)*K); 
			for(int i = 0; i < len1; i++)
	        ... // se realiza la suma
			*a = temp; // para poder guardar este valor en la dirección de a
		}
		...
		int arr**;
		colocar_memoria_y_sumar2dim(&arr,L,K); // para enviar la dirección de arr
		
```
***
[[Aritmética de punteros]]