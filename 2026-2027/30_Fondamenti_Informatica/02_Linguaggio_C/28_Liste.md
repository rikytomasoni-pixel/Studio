---
tags:
  - FI
  - programmazione-c
  - liste
  - nodi
  - strutture-dati
  - puntatori
  - struct
  - typedef
  - allocazione-dinamica
  - ricorsione
date: 2026-11-25
materia: Fondamenti di Informatica
fonte: Linguaggio C
---
# Liste

*Struttura dati dinamica fatta di nodi collegati tra loro da puntatori, allocati sull'heap con `malloc`.*

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
## Inserimento in Testa
```C
int inserisci_testa(lista_t* l, int v){
	nodo_t* nuovo; 
	nuovo = malloc(sizeof(nodo_t));
	if(!nuovo)
		return -1;
	nuovo->info = v; // come scrivere (*nuovo).info = v;
	nuovo->next = *l;
	*l = nuovo;
	return 0;
}
//versione che restituisce la nuova testa
lista_t inserisci_testa2(lista_t l, int v){
	nodo_t *nuovo;
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
	
	if(!(*l)) //lista vuota
		*l = nuovo;
	else{
		p = *l;
		while(p->next)
			p = p->next;
		
		p->next = nuovo;
	}
	return 0;
}

```
### Versione ricorsiva
```C
int inserisci_coda_ric(lista_t* l, int v){
	nodo_t* nuovo;
	if(!(*l)){ /*Caso Base: Lista Vuota*/
		nuovo = malloc(sizeof(nodo_t)); 
		if(!nuovo)
			return -1;
		nuovo->info = v;
		nuovo->next = NULL;
		*l = nuovo;
		return 0;
	}
	/*Caso Ricorsivo: lista con almeno un elemento*/
	return inserisci_coda_ric(&(*l)->next, v);
}
```

## Funzione stampa
```C
void stampa(lista_t l){
	while(l){
		printf("%d ", l->info);
		l = l->next;
	}
}
```

## Funzione Cerca
*restituisce un puntatore ad un nodo*
```C
nodo_t* cerca(lista_t l, int x){
	if(!l) /*Caso Base 1: Lista vuota*/
		return NULL;
	if(l->info == x)/*Caso Base 2: elemento trovato*/
		return l;
	/*Caso Ricorsivo*/
	return cerca(l->next, x);
}
```

## Cancellazione Lista
```C
void cancella_lista(lista_t* l){
	nodo_t* temp;
	while(*l){
		temp = (*l)->next;
		free(*l);
		*l = temp;
	}
}

```
## Inserimento in Posizione
```C
int inserisci_posizione(lista_t* l, int v, int pos){
	nodo_t *nuovo;
	nodo_t *current;
	nodo_t *previus;
	int i;
	
	 nuovo = malloc(sizeof(nodo_t));
	 if(!nuovo)
		return -1;
	nuovo->info = v;
	curr = *l;
	prev = NULL;
	i = 0;
	while(current && i < pos){
		previus = current;
		current = current->next;
		i++;
	}
	if(!previus) /*lista vuota->inserimento in testa*/
		*l = nuovo;
	else
		prev->next = nuovo;
	nuovo->next = current;
	
	return 0;
}
```

![[InserimentoPosizione.png]]
## Cancellazione per valore
```C
int cancella_valore(lista_t *l, int v){
	nodo_t *curr;
	nodo_t *prev;
	int cont;
	
	prev = NULL;
	curr = *l;
	cont = 0;
	while(curr) {
		if(curr->info == v) {
			if(!prev) { /*cancellazione primo elemento*/
				*l = curr->next;
				free(curr);
				curr = *l
			} else {
				/*cancellare nodo*/
				prev->next = curr->next;
				free(curr);
				curr = prev->next;
			}
			cont++;
		} else {
			prev = curr;
			curr = curr->next;
		}
	}
	return cont;
}
```
## Lista ordinata
```C
int ordinata(lista_t l) {
	if(!l)/*Caso base: lista vuota*/
		return 1;
	if(!(l->next))/*Caso base: lista di un nodo*/
		return 1;
	if(l->info > l->next->info)/*Caso base: non ordinata*/
		return 0;
	/*Caso Ricorsivo*/
	return ordinata(l->next);
}
```

## Note collegate
- [[00_MOC_FdI]]
- Precedente: [[27_Argomenti_da_Riga_di_Comando]]
- [[26_Allocazione_Dinamica_della_Memoria]] — `malloc`/`free` per creare e distruggere i nodi
- [[14_Struct]] — il nodo è una struct (`.` e `->`)
- [[13_Typedef]] — `typedef` per `nodo_t` e `lista_t`
- [[20_Puntatori]] — `next` è un puntatore; puntatore a puntatore (`lista_t*`) per modificare la testa
- [[23_Puntatori_a_Strutture]] — operatore `->`
- [[24_Ricorsione]] — `inserisci_coda_ric` e `cerca` ricorsive
- [[19_Sottoprogrammi_Funzioni]] — passaggio per indirizzo della lista
- [[16_Cicli_Iterativi]] — scorrimento con `while` in `stampa` e `cancella_lista`
- [[27_Argomenti_da_Riga_di_Comando]] — `main(int argc, char* argv[])` dell'esempio

#FdI/c/liste
