---
tags:
date: 2026-11-23
materia: Fondamenti di Informatica
fonte: Linguaggio C
---
# Allocazione dinamica della memoria

![[Pasted image 20261123134112.png|505]]

## Allocazione di un array con dimensione scelta dall'utente
- libreria <stdlib.h>
- **malloc**(dimensione in byte)
```C
int Statico[DIM];
int dim;
int *p;

scanf(" %d", &dim);
while(dim <= 0){
	printf("errore.\n");
	scanf(" %d", &dim);
}

//allocazione dinamica
p = malloc(dim * sizeof(int));
if(!p){
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
### Caso Matrici

**AGGIUNGI DISEGNO**

```C
int r, c, i;
int **m
scanf(" %d%d", &r, &c);
while(r <= 0 || c <= 0){
	printf("Errore\n");
	scanf(" %d%d", &r, &c);
}

//allocazione
m = malloc(r * sizeof(int*))
if(!m)
	return -1;
for(i = 0; i < r; i++){
	m[i] = malloc(c * sizeof(int));
	if(!m[i])
		retun -1;
}

//utilizzo

//deallocazione
for(i = 0; i < r; i++)
	free(m[i]);
free(m);
```

## Note collegate
- [[00_MOC_FdI]]

#materia/argomento/sottoargomento
