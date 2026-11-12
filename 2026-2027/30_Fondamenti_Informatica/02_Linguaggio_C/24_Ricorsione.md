---
tags:
  - ricorsione
  - funzioni
  - sottoprogrammi
  - record-di-attivazione
  - stack
  - array
  - puntatori
  - fibonacci
  - FI
  - programmazione-c
date: 2026-11-11
materia: Fondamenti di Informatica
fonte: Linguaggio C
---
# Ricorsività

*in matematica*
![[factRicorsivo.png]]

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

int fibonacci(int); //riceve l'indice i e restituisce l'i-esimo numero di Fibonacci

int main(){
	
	return 0;
}

int fibonacci(int i){
	if(i == 0)
		return 0;
	if(i == 1)
		return 1;
	return fibonacci(i - 1) + fibonacci(i - 2);	
}
//Complessità computazionale enorme (esponenziale), meglio la versione iterativa
```

## Esempio Massimo
``` C
#include <stdio.h>
int maxRicorsivo(int [], int);

int main(){
	return 0;
}

int maxRicorsivo(int lista[], int dim){
	int max;
	
	if(dim == 1)//caso base
		return lista[0];
		
	max = maxRicorsivo(lista, dim - 1);
	if(max > lista[dim - 1])
		return max;
	return lista[dim - 1];
}

```

## Esempio Massimo e Minimo
``` C
void massimo_minimo(int A[], int dim, int *max, int *min){
	if(dim == 1)
		*max = *min = *A;
	else{
		massimo_minimo(A + 1, dim - 1, max, min);
		if(*A > *max)
			*max = *A;
		else if(*A < *min)
			*min = *A;
	}
}
```
## Note collegate
- [[00_MOC_FdI]]
- [[19_Sottoprogrammi_Funzioni]] — record di attivazione e stack: ogni chiamata ricorsiva ne alloca uno
- [[20_Puntatori]] — puntatori `max`/`min` passati per indirizzo in `massimo_minimo`
- [[22_Puntatori_a_Array]] — `A + 1` per scorrere l'array
- [[09_Array_Monodimensionali]]
- [[15_Condizione_if_else]] — caso base e caso ricorsivo
- [[16_Cicli_Iterativi]] — alternativa iterativa (es. fattoriale, Fibonacci)
- [[23_Puntatori_a_Strutture]]

#FdI/c/ricorsione
