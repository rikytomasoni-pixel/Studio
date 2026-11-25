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

## Dichiarazione lista
```C
#include <stdio.h>
#include <stdlib.h>

typedef struct nodo_{
	int info;
	struct nodo_* next;
} nodo_t;

typedef nodo_t* lista_t;
```
## Inserimento in Testa (funzione)
*implementazione poi*
```C
int inserisci_testa(lista_t* l, int v){
	nodo_t* nuovo; 
	nuovo = malloc(sizeof(nodo_t));
	if(!nodo)
		return -1;
	nuovo->info = v; // come scrivere (*nuovo).info = v;
}
lista_t inserisci_testa2(lista_t l, v){
	nodo_t *nodo;
	nuovo = malloc(sizeof(nodo_t));
	if(!nuovo)
		return l;
	nuovo->info = v;
	nuovo->next = l;
	return nuovo;
}
```
## Inserimento in Coda
```C
int inserisci_coda(lista_t* l, int v){
	nodo_t* nuovo;
	nodo_t* p;
	nuovo = malloc(sizeof(nodo_t));
	if(!nuovo)
		return -1;
	nuovo->info = v;
	nuovo->next = NULL;
	
	p = *l;
	while(p->next)
		p = p->next;
	
	p->next = nuovo;
	return 0;
}

```
## Applicazione tipo
```C
#include <stdio.h>
#include <stdlib.h>

typedef struct nodo_{
	int info;
	struct nodo_* next;
} nodo_t;

typedef nodo_t* lista_t;

int inserisci_testa(lista_t*, int);

int main(int argc, char* argv[]){
	lista_t l = NULL; //lista vuota
	
	inserisci_testa(&l, 3);
	return 0;
}

int inserisci_testa(lista_t* l, int v){
	nodo_t* nuovo; 
	nuovo = malloc(sizeof(nodo_t));
	if(!nodo)
		return -1;
	nuovo->info = v; // come scrivere (*nuovo).info = v;
	nuovo->next = *l
	*l = nuovo;
	return 0;
}
```
## Note collegate
- [[00_MOC_Materia]]

#materia/argomento/sottoargomento
