---
tags:
  - funzioni
  - array
  - puntatori
  - tipi-di-dato
  - indirizzi-di-memoria
date: 2026-11-09
materia: Fondamenti di Informatica
fonte:
---
# Utilizzo di Array nelle funzioni

``` C
#include <stdio.h>
#define DIM 5

void Stampa(int *, int); //posso scrivere anche int [] invece che int **
int main() {
	int A[5] = {1, 2, 3, 4, 5};
	Stampa(A, DIM);
	
	return 0;
}

void Stampa(int *v, int n){ 
	int i;
	for()
}
```

## Note collegate
- [[00_MOC_FdI]]

#materia/argomento/sottoargomento
