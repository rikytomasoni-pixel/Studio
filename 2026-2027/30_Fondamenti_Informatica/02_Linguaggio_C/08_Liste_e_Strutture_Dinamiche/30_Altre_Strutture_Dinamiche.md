---
tags:
  - FI
  - programmazione-c
  - strutture-dati
  - liste-doppie
  - liste-circolari
  - alberi
  - grafi
date: 2026-11-25
materia: Fondamenti di Informatica
fonte: Linguaggio C
---
# Altre strutture dinamiche

- Abbiamo visto le liste concatenate: [[28_Liste]]
- **Liste doppiamente concatenate**: ogni nodo ha anche il puntatore al nodo precedente
```C
typedef struct nodo_{
	int info;
	struct nodo_ *next;
	struct nodo_ *prev;
} nodo_t;
```

![[concatenate.png]]
- **Liste circolari**
![[circolari.png]]
- **Alberi**
![[alberi.png]]
- **Grafi**
![[Grafi.png]]

## Schema di riepilogo

![[schemaUsoStruttureDati.pdf]]

## Note collegate
- [[00_MOC_FdI]]
- Precedente: [[29_Programmazione_Modulare]]
- [[28_Liste]] — lista concatenata semplice
- [[14_Struct]] — i nodi sono struct autoreferenziali
- [[26_Allocazione_Dinamica_della_Memoria]] — i nodi vivono sull'heap

#FdI/c/strutture-dinamiche
