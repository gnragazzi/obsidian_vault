```
Rec_BinarySearch(List,lower,upper,X)
	{
	 Look for X in List[lower..upper]
	 Report position if found, else report 0
	 List is Sorted in increasing order.
	 0<lower≤upper. 
	}
	if lower = upper then
		if x=List[lower] then
			return lower
		else
			return 0
	else
		mid <- ceil((lower + upper)/2)
		if (x>List[mid])
			then 
				return RecBinarySearch(List,mid+1,upper,X)
			else
				return RecBinarySearch(List,lower,mid,X)
```
***
[Compared to What?]
Esta es la versión que en la materia vimos como bi-sección.