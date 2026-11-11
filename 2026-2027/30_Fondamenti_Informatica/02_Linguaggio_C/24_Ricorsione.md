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
	printf("%d\n", fattorialeRicorsivo(4));
	return 0;
}

int fattorialeRicorsivo(int n){
	if(n == 0) //caso base
		return 1;
	return n * fattorialeRicorsivo(n - 1); //caso ricorsivo
}
```

## Esempio Fibonacci

``` C
#include <stdio.h>

int fibonacci(int); //riceve l'indice i esimo restituisce il numero i esimo

int main(){
	
	return 0;
}

int fibonacci(int i){
	if(i == 0)
		return 0;
	if(i == 1)
		return 1;
	return fibonacci(i - 1) + fibonacci(i -2);
	
}
```

## Note collegate
- [[00_MOC_FdI]]

#materia/argomento/sottoargomento
