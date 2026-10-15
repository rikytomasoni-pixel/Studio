---
tags:
  - FI
  - programmazione-c
  - array
date: 2026-09-24
materia: Fondamenti di Informatica
fonte: Linguaggio C
---

# Array/Vettori

Tipo di dato composto il cui scopo è ospitare una collezione di variabili dello stesso tipo (collezione di dati omogenei)

## Monodimensionali

```C
#include <stdio.h>
#define DIM 5
int main(){
	//tipo NomeVariabile[COSTANTE_INTERA];
	int Array[DIM];
```

**Accesso ai componenti/elementi dell'Array**
- **Accesso posizionale** [0,1,...,DIM-1]
```C
Array[2] = 4; //nella terza cella inserisco 4

scanf("%d",&Array[0]);

Array[3]=Array[2]*Array[2];

i=Array[2]/2;
Array[i]=Array[i+1];

Array[0]=2;
Array[Array[0]]++;

Array[5]=4; //ERRORE: Accesso fuori Array
/*compila ma potrebbe intaccare zone di memoria
non previste e portare alla terminazione del programma*/
```

- **Input/Output e navigazione Array**
```C
int A[DIM],B[DIM];
int i,uguali;

for(int i=0;i<DIM;i++)
	scanf("%d",&A[i]);
	
for(int i=0;i<DIM;i++)
	printf("%d\n",A[i]);

/*controllo uguaglianza*/
uguali=1;
for(int i=0;i<DIM&&uguali;i++)
	if(A[i]!=B[i])
		uguali=0;
```

## Note collegate
- [[00_MOC_FdI]]
- Precedente: [[08_Conversione_fra_Tipi]]
- Successiva: [[10_Stringhe_in_C]]

#FdI/c/array
