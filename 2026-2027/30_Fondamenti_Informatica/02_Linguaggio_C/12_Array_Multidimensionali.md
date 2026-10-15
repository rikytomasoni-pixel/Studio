---
tags:
  - FI
  - programmazione-c
  - array
  - matrici
date: 2026-09-24
materia: Fondamenti di Informatica
fonte: Linguaggio C
---

# Array multidimensionali

```C
int matrice [Righe][Colonne];
int tridim[Strato][Righe][Colonne];

matrice[1][2]=2;

for(int i=0;i<Righe;i++)
	for(int j=0;j<Colonne;j++)
		istruzione;
		
```

## Salvataggio in memoria

Le matrici in C vengono salvate in maniera lineare detta *Row Major Order*
- **i** indice di riga
- **j** indice di colonna

Vedi anche gli [[11_Operazioni_sulle_Stringhe|array di stringhe]] (matrice di char).

## Note collegate
- [[00_MOC_FdI]]
- Precedente: [[11_Operazioni_sulle_Stringhe]]
- Successiva: [[13_Typedef]]

#FdI/c/array-multidimensionali
