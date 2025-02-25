- Apertura
```
	FILE *fp = fopen(char nom[],char metodo);
```
- Clausura
	```
	fclose(FILE *fp);
	```
- Lectura
	- Caracter
		```
		fgetc(FILE *);//retorna el char al que apunta fp y mueve el puntero
		fputc(char, FILE *); posiciona el caracter y mueve el puntero
		```
		
+ Escritura
	+ Para escribir un archivo, como se imprime por pantalla, se utiliza 
		+ ```fprintf(FILE*, char * format, ...)```
			+ donde `format` contiene una cadena (del tipo de las usadas en printf). 
			+ `...` es un número arbitrario de argumentos, según lo que se haya escrito en `format`