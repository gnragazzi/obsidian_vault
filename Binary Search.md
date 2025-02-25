```
BinarySearch(List,lower,upper,X)
	{
	 Look for X in List[lower..upper]
	 Report position if found, else report 0
	 List is Sorted in increasing order.
	 0<lower≤upper. 
	}
	while lower ≤ upper
		mid <- ceil((lower+upper)/2)
		case List[mid]
			< X :
				low <- mid + 1
			= X : 
				return mid
			> z :
				upper <- mid - 1
	return 0
```
***
[[Peor costo para la Búsqueda Binaria]]
***
- [[Versión Recursiva de Búsqueda Binaria]]:



