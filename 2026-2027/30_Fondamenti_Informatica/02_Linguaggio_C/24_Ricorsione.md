---
tags:
date: 2026-11-11
materia: Fondamenti di Informatica
fonte: Linguaggio C
---
# Ricorsività

*in matematica*
![[Pasted image 20261111085747.png]]

*in C*
``` C
#include <stdio.h>

int fattorialeRicorsivo(int);

int main(){
	printf("")
	return 0;
}

int fattorialeRicorsivo(int n){
	if(n == 0) //caso base
		return 1;
	return n * fattorialeRicorsivo(n - 1); //caso ricorsivo
}
```

## Note collegate
- [[00_MOC_FdI]]

#materia/argomento/sottoargomento
