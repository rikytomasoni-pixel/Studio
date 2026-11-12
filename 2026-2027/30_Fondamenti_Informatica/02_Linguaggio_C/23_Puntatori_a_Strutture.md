---
tags:
  - puntatori
  - struct
  - indirizzi-di-memoria
  - tipi-definiti-dall-utente
  - tipi-di-dato
  - FI
  - programmazione-c
date: 2026-11-09
materia: Fondamenti di Informatica
fonte: Linguaggio C
---
# Puntatori a Strutture

``` C
#define MAX 50
typedef struct {
	char cognome[MAX + 1];
	char nome[MAX + 1];
	int matricola;
} studente_t;
void stampa(studente_t);
void stampa2(studente_t);
```

```C
int main(){
	studente_t stud = {"Rossi", "Mario", 123456};
	studente_t *ptr;
	ptr = &stud;
	
	printf("%s\n", (*ptr).cognome);
	printf("%s\n", ptr->cognome); //operatore freccia
	
	stampa(stud);
	stampa2(&stud); //passaggio per indirizzo: non si copia la struct
	
	return 0;
}
```

```C
//le strutture in C sono passate per valore (si copia tutta la struct)
void stampa(studente_t s){ 
	printf("%s\n", s.cognome);
	printf("%s\n", s.nome);
	printf("%d\n", s.matricola);
}
```

```C
void stampa2(studente_t *s){
	printf("%s\n", s->cognome); //operatore freccia
	printf("%s\n", s->nome);
	printf("%d\n", s->matricola);
}
```
## Note collegate
- [[00_MOC_FdI]]
- [[20_Puntatori]]
- [[05_Tipi_di_Dato]]
- [[14_Struct]]
- [[13_Typedef]]
- [[19_Sottoprogrammi_Funzioni]]
- [[22_Puntatori_a_Array]]
- [[24_Ricorsione]]
- [[10_Stringhe_in_C]]

#FdI/c/puntatori-strutture
