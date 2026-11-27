---
tags:
  - FI
  - programmazione-c
  - stringhe
  - string.h
date: 2026-09-24
materia: Fondamenti di Informatica
fonte: Linguaggio C
---

# Operazioni sulle stringhe

Serve la libreria `#include <string.h>`

- calcolo della lunghezza
```C
//trattarlo come array ed usare contatore

char str[] = {"ciao"};
int lunghezza;
lunghezza = strlen(str);
```
- copia
```C
int i;
char str[5] = {"ciao"};
char str2[5];

for(i = 0; str[i] != '\0'; i++)
	str2[i] = str[i];
str2[i] = '\0';

len = strlen(str);
for(i = 0; i < len; i++)
	str2[i] = str[i];
	
strcpy(str2, str);
```
- confronto
```C
char str[] = {"ciao"};
char str2[] = {"ciao"};
res = strcmp(str, str2);
/*
res=0 se le stringhe sono uguali (caratteri prima del terminatore)
res<0 se str è alfabeticamente minore di str2
res>0 se str è alfabeticamente maggiore di str2

la relazione d'ordine per l'alfabeto fa riferimento al codice ASCII 'a'<'b'
"aa"<"ab"
*/
```
- concatenazione 
```C
strcat(str, str2); //aggiunge in str la stringa str2
```

## Array di stringhe

- matrice di char
```C
char arrayStringhe[N_STRINGHE][DIM + 1];
int i;

for(i = 0; i < N_STRINGHE; i++)
	scanf("%s", arrayStringhe[i]);

for(i = 0; i < N_STRINGHE; i++)
	printf("%s\n", arrayStringhe[i]);
```

## Note collegate
- [[00_MOC_FdI]]
- Precedente: [[10_Stringhe_in_C]]
- Successiva: [[12_Array_Multidimensionali]]

#FdI/c/operazioni-stringhe
