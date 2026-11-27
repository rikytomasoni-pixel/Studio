---
tags:
  - FI
  - programmazione-c
  - argc
  - argv
  - riga-di-comando
  - stringhe
  - atoi
  - atof
date: 2026-11-23
materia: Fondamenti di Informatica
fonte: Linguaggio C
---
# Argomenti da riga di comando

*Passare dati a un programma al momento dell'esecuzione, come parametri del `main`.*

- `int argc`
	- arguments counter: numero di argomenti
- `char* argv[]`
	- arguments values: vettore di stringhe con i valori degli argomenti

## Funzioni da libreria
Servono a convertire gli argomenti (che sono sempre stringhe) in numeri.
- `atoi`
```C
int atoi(char*); //ascii to int
```
- `atof`
```C
float atof(char*); //ascii to float
```

> [!note] Osservazione (non presente negli appunti)
> `argv[0]` contiene il nome del programma, quindi gli argomenti passati dall'utente sono `argv[1]`, ..., `argv[argc - 1]` e `argc` vale almeno 1. Esempio minimo:
> ```C
> int main(int argc, char* argv[]){
> 	if(argc < 2)
> 		return -1;
> 	int n = atoi(argv[1]); //da stringa a intero
> 	return 0;
> }
> ```
> Le funzioni `atoi`/`atof` sono dichiarate in `<stdlib.h>`.

## Note collegate
- [[00_MOC_FdI]]
- Precedente: [[26_Allocazione_Dinamica_della_Memoria]]
- [[10_Stringhe_in_C]] — ogni elemento di `argv` è una stringa (array di `char` terminato da `\0`)
- [[19_Sottoprogrammi_Funzioni]] — `main` è una funzione con parametri
- [[20_Puntatori]] — `char* argv[]` è un array di puntatori a `char`
- [[22_Puntatori_a_Array]] — array di puntatori e aritmetica
- [[08_Conversione_fra_Tipi]] — `atoi`/`atof` convertono stringa → numero
- [[03_Struttura_di_un_Programma_C]] — struttura del `main`
- Successiva: [[28_Liste]]

#FdI/c/argomenti-riga-comando
