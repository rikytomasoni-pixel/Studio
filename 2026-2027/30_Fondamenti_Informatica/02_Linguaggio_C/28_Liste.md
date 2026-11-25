---
tags:
date: 2026-11-25
materia: Fondamenti di Informatica
fonte: Linguaggio C
---
# Liste

![[tabella_liste.png|616]]

Un elemento di una lista si chiama **NODO**
Un nodo è formato dall'**informazione** e dal **puntatore** al nodo successivo

![[StrutturaNodi.png]]

## Dichiarazione lista vuota
```C
#include <stdio.h>
#include <stdlib.h>

typedef struct nodo_{
	int info;
	struct nodo_* next;
} nodo_t;

typedef nodo_t* lista_t;

int main(int argc, char* argv[]){
	lista_t l = NULL; //lista vuota
	return 0;
}
```
## Inserimento in Testa (funzione)
*implementazione poi*
```C
int inserisci_testa(lista_t* l, int v){ //esempio inserisci_testa(&l, 3)
	nodo_t* nuovo; 
	nuovo = malloc(sizeof(nodo_t));
}
```
## Note collegate
- [[00_MOC_Materia]]

#materia/argomento/sottoargomento
