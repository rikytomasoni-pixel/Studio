---
tags:
  - FI
  - programmazione-c
  - struct
  - tipi-definiti-dall-utente
date: 2026-09-24
materia: Fondamenti di Informatica
fonte: Linguaggio C
---

# Strutture/Struct

Collezione di dati eterogenei
```C
#define DIM 50
#define N_ESAMI 30

//dichiarazione di un singolo dato struttura
struct{//tipo di dato
char nome[DIM + 1];//campi
char cognome[DIM + 1];
unsigned int voti[N_ESAMI];
}studente;//identificatore

//accesso con dot notation
//identificatore.nome
studente.nome;

//Variabili struct precostruite
typedef struct{//tipo di dato
char nome[DIM + 1];//campi
char cognome[DIM + 1];
unsigned int voti[N_ESAMI];
}studente_t;//identificatore

//struct annidate
typedef struct{
unsigned int giorno;
unsigned int mese;
unsigned int anno;
}data_t;

typedef struct{//tipo di dato
char nome[DIM + 1];//campi
char cognome[DIM + 1];
unsigned int voti[N_ESAMI];
data_t dataNascita;
}studente_t;//identificatore

studente_t mario, paolo;

//operazioni tipo
int giornoMario = mario.dataNascita.giorno;
paolo = mario;

//array di tipi studente
studente_t classe[DIM];
```

Per la definizione di nuovi nomi di tipo vedi [[13_Typedef]].

## Note collegate
- [[00_MOC_FdI]]
- Precedente: [[13_Typedef]]
- Successiva: [[15_Condizione_if_else]]

#FdI/c/struct
