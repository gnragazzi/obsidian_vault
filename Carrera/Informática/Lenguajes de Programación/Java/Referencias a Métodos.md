`Referencia::NombreMétodo`
por ejemplo:
- var->System.out.println(var) equivale a System.out::println
***
Son muy utilizadas en consonancia con [[Stream API|streams]], por ejemplo:
```
import java.util.ArrayList;  
  
public class Ejercicio {  
    public static void main(String[] args){  
        ArrayList<Integer> intList = new ArrayList<>();  
        intList.add(1);  
        intList.add(2);  
        intList.add(3);  
  
        for(int i : intList){ System.out.println(i); }  
        intList.stream().map((x)->x+1).forEach(System.out::println);  
  
        for(int i : intList){ System.out.println(i); }  
  
    }  
}
```



