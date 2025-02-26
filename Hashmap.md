Se recorre utilizando el tipo Map.Entry:
```
for (Map.Entry<K,V> identif_en_loop : identificador.entrySet() ){
	K clave = identif_en_loop.getKey();
	V value = identif_en_loop.getValue();
	{...}
}
```