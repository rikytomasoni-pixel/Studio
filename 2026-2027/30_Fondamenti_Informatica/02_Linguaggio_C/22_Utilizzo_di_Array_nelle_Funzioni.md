---
tags:
  - funzioni
  - array
  - puntatori
  - tipi-di-dato
  - indirizzi-di-memoria
date: 2026-11-09
materia: Fondamenti di Informatica
fonte: Linguaggio C
---
# Utilizzo di Array nelle funzioni
## Monodimensionali
``` C
#include <stdio.h>
#define DIM 5

void Stampa(int *, int); //posso scrivere anche int [] invece che int *
int main() {
	int A[5] = {1, 2, 3, 4, 5};
	Stampa(A, DIM);
	
	return 0;
}

void Stampa(int *v, int n){ //posso scrivere anche int v[] invece che *v
	int i;
	for(i = 0; i < DIM; i++)
		printf("%d\n", *(v + i)); //posso scrivere anche v[i] invece che *(v + i)
}
```
## Multidimensionali
``` C
#define R 2
#define C 3

double

```

## Note collegate
- [[00_MOC_FdI]]
- [[20_Puntatori]]
- [[19_Sottoprogrammi_Funzioni]]
- [[12_Array_Multidimensionali]]

#materia/argomento/sottoargomento
