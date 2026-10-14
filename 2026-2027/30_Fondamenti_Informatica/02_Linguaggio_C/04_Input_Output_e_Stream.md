---
tags:
  - FI
  - programmazione-c
  - input-output
  - scanf
  - printf
date: 2026-09-24
materia: Fondamenti di Informatica
fonte: Linguaggio C
---

# Funzioni IN → OUT

```c
#include <stdio.h>  // libreria
```

Caratteri di formato / di conversione: `%f`, `%d`, `%c`, etc

La gestione di stdin è basata sullo **stream o flusso**. Lo scanf cerca nello stream valori associabili a quelli ricercati (*pattern matching*). Le informazioni che rimangono nel buffer (architettura dello stream) possono dare vita a problemi di buffering dell'input.

```C
scanf("%c",&val);
fflush(stdin);
scanf("%c",&val1);

scanf("%c ",&val);
scanf("%c",&val1);

scanf("%c",&val);
scanf(" %c",&val1);

scanf("%c %c",&val,&val1);

scanf("%c",&val);
scanf("%c");
scanf("%c",&val1);
```

## Note collegate
- [[00_MOC_FdI]]
- Precedente: [[03_Struttura_di_un_Programma_C]]
- Successiva: [[05_Tipi_di_Dato]]

#FdI/c/input-output
