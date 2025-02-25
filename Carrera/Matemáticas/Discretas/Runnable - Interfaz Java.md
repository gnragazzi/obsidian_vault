Es la forma más fácil de crear un thread en Java.
Para implementar runnable hay que 
- instanciar `Thread`, cuyo constructor aceptara una clase que implemente `Runnable` como primer parámetro. Está instanciación es naturalmente hecha en el constructor
- Tener un atributo privado de clase Thread;
- re-definir el método `public void run()` donde van todas las instrucciones del thread
Ejemplo: 
```
public class RunImplClass implements Runnable{
    private Thread t; // de esta forma, el thread está encapsulado en la clase que implementa Runnable
    
    public RunImplClass(String name){
        t = new Thread(this,name); // se crea el thread en el constructor, y se lo asigna al atributo privado.
    }
    public void run(){
		 // Lo que hará el thread
    }
    
    public void threadStart(){
        this.t.start();    
    }
    ...
}
```