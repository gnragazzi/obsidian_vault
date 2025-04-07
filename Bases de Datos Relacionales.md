1. Parte 1
	1. Clase
		1. [[Teorema de CAP]] 
		2. [[Diagrama Entidad Relación]]
	2. Vivo
		1. [[Primary Key]]
		2. [[Foreign Key]]
2. Consultas SQL parte 2
	1. Clase
		1. DDL
			1. Create
			2. ALTER
			3. DROP
		2. DML
			1. SELECT
				1. SELECT col_1,col_2 FROM table;
					1. where cond;
					2. ORDER BY campo (asc|desc);
					3. LIMIT cant_reg;
					4. DISTINCT // solo tuplas no repetidas
			2. INSERT
				1. INSERT INTO nom_tabla VALUES(val_para_col);
			3. UPDATE
				1. UPDATE tabla SET nom_atr=val WHERE cond;
			4. DELETE
				1. DELETE FROM tabla WHERE cond;
		3. OPERADORES
			1. RELACIONALES
			2. LIKE / NOT LIKE
				1. patrón específico en una columna de tipo string
				2. Reempla el operador de igualdad
			3. BETWEEN
				1. min AND max
		4. Funciones de agregación
			1. COUNT
			2. MIN
			3. MAX
				1. SELECT MAX(campo),(campos opcionales) FROM tabla;
			4. SUM 
			5. AVG
		5. BUENAS PRÁCTICAS
			1. Evitar SELECT *
			2. Evitar consultas sin filtros o límites de registros
			3. No se recomienda ORDER BY para consultas con grandes volúmenes de datos.
			4. Cuando una consulta va con varias tablas, aclarar a que tabla corresponde cada atributo.
	2. Vivo
		1. 
3. Consultas SQL avanzadas parte 1
	1. Clase
	2. Vivo
4. Optimización de Bases de Datos parte 2
	1. Clase
	2. Vivo