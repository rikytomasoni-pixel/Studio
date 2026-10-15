---
tags:
  - FI
  - programmazione-c
  - stringhe
  - array
date: 2026-09-24
materia: Fondamenti di Informatica
fonte: Linguaggio C
---

# Stringhe in C

- array di char

![[CarattereTerminatore.png]]

- Dimensione -> 9
- Lunghezza -> 4 (il terminatore `\0` non viene contato)

## Lettura e scrittura

```C
#include <stdio.h>
#define DIM 20
int main(){
	char str[DIM];
	scanf("%s", str) //%s e non va messa &
	// legge finché non incontra o " " o "\n"
	scanf("%[^\n]",str); //legge sequenza di caratteri finché non incontra "\n"
	//whitelist-blacklist (^ = NOT)
	return 0;
}
```

Le operazioni sulle stringhe sono descritte in [[11_Operazioni_sulle_Stringhe]].

## Note collegate
- [[00_MOC_FdI]]
- Precedente: [[09_Array_Monodimensionali]]
- Successiva: [[11_Operazioni_sulle_Stringhe]]
- Disegno originale: [[Disegni FI]]

#FdI/c/stringhe
