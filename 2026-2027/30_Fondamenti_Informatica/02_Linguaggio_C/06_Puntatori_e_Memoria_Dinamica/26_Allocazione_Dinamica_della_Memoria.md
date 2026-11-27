---
tags:
  - FI
  - programmazione-c
  - allocazione-dinamica
  - malloc
  - calloc
  - realloc
  - free
  - heap
  - puntatori
  - array
  - matrici
date: 2026-11-23
materia: Fondamenti di Informatica
fonte: Linguaggio C
---
# Allocazione dinamica della memoria

*Richiedere memoria sull'heap durante l'esecuzione, con dimensione decisa a runtime (ad esempio dall'utente), tramite la libreria `<stdlib.h>`.*

![[allocazioneDinamica.png|505]]

## Allocazione di un array con dimensione scelta dall'utente
- libreria `<stdlib.h>`
- **malloc**(dimensione in byte)
```C
int Statico[DIM]; //array statico: dimensione fissa decisa a tempo di compilazione
int dim;
int *p;

scanf(" %d", &dim);
while(dim <= 0){
	printf("errore.\n");
	scanf(" %d", &dim);
}

//allocazione dinamica
p = malloc(dim * sizeof(int));
if(!p){ //malloc restituisce NULL se l'allocazione fallisce
	printf("errore.\n");
	return -1;
}
//utilizzo p come se fosse un array normale
for(int i = 0; i < dim; i++){
	scanf(" %d", &p[i]);
}
//deallocazione
free(p);
```

### Caso matrici
![[MatriciDinamiche.png]]

```C
int r, c, i;
int **m;
scanf(" %d%d", &r, &c);
while(r <= 0 || c <= 0){
	printf("Errore\n");
	scanf(" %d%d", &r, &c);
}

//allocazione
m = malloc(r * sizeof(int*));
if(!m)
	return -1;
for(i = 0; i < r; i++){
	m[i] = malloc(c * sizeof(int));
	if(!m[i])
		return -1;
}

//utilizzo

//deallocazione
for(i = 0; i < r; i++)
	free(m[i]);
free(m);
```

### Allocazione con funzione
```C
int* alloca_array(int dim){
	int *p2;
	p2 = malloc(dim * sizeof(int));
	return p2;
}
```

## Altre funzioni
- **calloc**(numero elementi, dimensione elementi)
	- alloca e inizializza tutti i byte a 0
```C
p = calloc(dim, sizeof(int));
```
- **realloc**(array, dimensione)
	- ridimensiona l'array
	- potrebbe fallire: per questo non si sovrascrive mai direttamente il puntatore originale (si perderebbe l'indirizzo del blocco e non si potrebbe più fare `free`)
	- potrebbe spostare l'array in un altro indirizzo di memoria, a seconda dell'occupazione dell'heap
```C
p2 = realloc(p, 3 * dim * sizeof(int));
if(!p2)
	printf("riallocazione fallita\n");
else
	p = p2;
//corpo
free(p);
```

## Note collegate
- [[00_MOC_FdI]]
- Precedente: [[25_Gestione_File]]
- Successiva: [[27_Argomenti_da_Riga_di_Comando]]
- [[20_Puntatori]] — il risultato di `malloc` è un puntatore; `NULL` e dereferenziazione
- [[22_Puntatori_a_Array]] — `p[i]` equivale a `*(p + i)`: il blocco allocato si usa come array
- [[09_Array_Monodimensionali]] — array statici (dimensione fissa) vs dinamici
- [[12_Array_Multidimensionali]] — matrici statiche vs matrice dinamica come array di puntatori
- [[07_sizeof_e_Librerie_limits_float]] — `sizeof` per calcolare i byte da allocare
- [[19_Sottoprogrammi_Funzioni]] — funzione che restituisce un puntatore (`alloca_array`)
- [[21_Regole_di_Visibilità]] — la memoria dinamica sopravvive alla funzione che la alloca, a differenza delle variabili locali
- [[14_Struct]] — si possono allocare dinamicamente anche array di struct
- [[15_Condizione_if_else]] — controllo `if(!p)` dopo ogni allocazione
- [[28_Liste]] — nodi allocati dinamicamente

#FdI/c/allocazione-dinamica
