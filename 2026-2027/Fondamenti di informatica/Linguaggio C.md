---
tags:
  - codifica
  - algoritmi
  - informatica
  - programmazione-c
  - FI
date: 2026-09-24
materia: Fondamenti di Informatica
---

# Linguaggi di Programmazione

Un linguaggio di programmazione è un linguaggio formale caratterizzato da una propria **sintassi** e **semantica**.
## Livelli del linguaggio
I linguaggi di programmazione possono essere di **alto livello** (più simili al linguaggio naturale) o di **basso livello** (più simili al *linguaggio macchina*)

`Problema` → `Algoritmo` → `Programma
## Compilati vs Interpretati

Un linguaggio di programmazione può diventare linguaggio macchina attraverso 2 processi la **compilazione** e l'**interpretazione**. La prima si passa dal *codice sorgente* attraverso la *compilazione* ad un *programma eseguibile*, il secondo invece esegue il codice sorgente **riga per riga**.

Esistono eccezioni come ad esempio java che compila un bytecode e poi lo interpreta

# Il linguaggio C

C → Denis Ritchie anni '60 (ANSI 89)

![[Struttura codice C.png]]
## Dichiarazioni variabili

- nome (identificazione)
- tipo → fortemente tipizzato
- Case sensitive

## Dichiarazioni costanti

```c
#define NOME ...
```

## Funzioni IN → OUT

```c
#include <stdio.h>  // libreria
```

Caratteri di formato / di conversione: `%f`, `%d`, `%c`, etc

La gestione di stdin è basata sullo **stream o flusso**. Lo scanf cerca nello stream valori associabili a quelli ricercati (*pattern matching*). Le informazioni che rimangono nel buffer (architettura dello stream) posso dare vita a problemi di buffering dell'input.

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
---

# Tipi di dato

- Predefiniti (Built-in)
- Definiti dall'utente (user-defined)

- semplici
- composti

## Dati predefiniti e semplici

### INT → numeri interi con segno

- Complemento a 2
- tipicamente 32 bit (4 byte)
- $[-2^{31},\ 2^{31}-1]$
- operazioni aritmetiche: `+`, `*`, `-`, `/`, `%`
- Lettura-scrittura `%d`
- Varianti:
	- `unsigned int` → `unsigned int y;` → `%u` → binario naturale
	- `short`, `long` → numeri interi con segno, tipicamente 16 bit / 64 bit

### CHAR → caratteri

- 8 bit (1 byte) → $[0,\ 255]$
- codifica ASCII
- `%c`
- operazioni

### FLOAT → numeri razionali

- virgola mobile in singola precisione
- IEEE 754 → 32 bit
- operazioni NO `%`

### DOUBLE → numeri razionali

- virgola mobile in doppia precisione
- IEEE 754 → 64 bit
- `scanf` → `%lf`
- `printf` → `%f`

#### sizeOf

`sizeof(int)` → # byte occupati da una variabile di tipo `int`

#### Librerie

`<limits.h>`
- `INT_MAX` → max valore rappresentabile con `int`
- `INT_MIN`
- `UINT_MAX`
- `UINT_MIN`

`<float.h>`
- `FLT_MAX`
- `FLT_MIN`
- `FLT_EPS`
- `DBL_MAX`
- `DBL_MIN`
- `DBL_EPS`

#### Conversione fra tipi

→ gerarchia basata sul potere rappresentativo

Conversione per promozione / retrocessione (→ / ←)

Conversione implicita e esplicita:
- **implicita**: assegno un valore in una variabile di gerarchia diversa
- **esplicita**: CASTING → `(tipo)espressione`
## Dati Composti

### Array/Vettori
Tipo di dato composto il cui scopo è ospitare una collezione di variabili dello stesso tipo (collezione di dati omogenei)

#### Monodimensionali
```C
#include <stdio.h>
#define DIM 5
int main(){
	//tipo NomeVariabile[COSTANTE_INTERA];
	int Array[DIM];
```
##### Accesso ai componenti/elementi dell'Array
- **Accesso posizionale** [0,1,...,DIM-1]
```C
Array[2] = 4; //nella terza cella inserisco 4

scanf("%d",&Array[0]);

Array[3]=Array[2]*Array[2];

i=Array[2]/2;
Array[i]=Array[i+1];

Array[0]=2;
Array[Array[0]]++;

Array[5]=4; //ERRORE: Accesso fuori Array
/*compila ma potrebbe intaccare zone di memoria
non previste e portare alla terminazione del programma*/
```

- **Input/Output e navigazione Array**
```C
int A[DIM],B[DIM];
int i,uguali;

for(int i=0;i<DIM;i++)
	scanf("%d",&A[i]);
	
for(int i=0;i<DIM, i++)
	printf("%d\n",A[i]);

/*controllo uguaglianza*/
uguali=1;
for(int i=1;i<DIM&&uguali;i++)
	if(A[i]!=B[i])
		uguali=0;
```
#### Stringhe in C
- array di char
![[CarattereTerminatore.png]]

- Dimensione -> 9
- Lunghezza -> 4 (considerare il terminatore)
##### Lettura e scrittura
```C
#include <stidio.h>
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
##### Operazioni sulle stringhe
Serve la libreria ```#include <string.h```
- calcolo della lunghezza
```C
//trattarlo come array ed usare contatore

str[] = {"ciao"};
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
for(i = 0; str[i] < len; i++)
	str2[i] = str[i];
	
strcpy(str2, str);
```
- confronto
```C
char str = {"ciao"};
char str2 = {"ciao"};
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
#### Multidimensionali 
```C
int matrice [Colonne][Righe];
int tridim[Colonne][Righe][Strato];

matrice[1][2]=2;

for(int i=0;i<Colonne;i++)
	for(int j=0;j<Righe;j++)
		istruzione;
		
```
##### Salvataggio in memoria
Le matrici in C vengono salvate in maniera lineare detta *Row Major Order*
- **i** indice di riga
- **j** indice di colonna
##### Array di stringhe
- matrice di char
```C
char arrayStringhe[N_STRINGHE][DIM + 1];
int i;

for(i = 0; i < N_STRINGHE; i++)
	scanf("%s", arrayStringhe[i]);

for(i = 0; i < N_STRINGHE; i++)
	printf("%s\n", arrayStringhe[i]);
```
### Strutture/Struct
Collezione di dati eterogenei

---

# Condizione if-else

## Operatori relazionali

`>=`, `<=`, `!=`, `>`, `<`, `==

## Operatori logici

- AND → `&&`
- OR → `||` ("pipe")
- NOT → `!`

In C è falsa ogni espressione che valuta $0$ ed è vera qualsiasi altro valore $\neq 0$.

# Cicli iterativi
## Pre-condizione

```C
while(true){
	...
}
```

## Post-condizione

```C
do{
	...
}while(true);
```


> [!NOTE] Abbreviazioni
> a=b=1;
> *Operatori di auto-incremento*
> i++ (post-incremento), ++i (pre-incremento)
> *Operatori di auto-decremento*
> i-- (post-decremento), --i (pre-decremento)
> *Altri*
> i+=j
> i*=j
> i-=j
> i/=j
> i%=j

## Iterazione definita

```C
for(istruzioniDiInizializzazione; condizione; istruzioniDiIncrementoDecremento){
	...
}
```
### Excursus sui numeri di Kaprekar
```C

/* Determinare se un numero intero è un numero di Kaprekar,
cioè se il suo quadrato diviso in 2 porzioni, eventualmente vuote, che,
sommate tra loro danno il numero
45^2=2025 e 20+25=45
*/

#include <stdio.h>
#include <math.h>

int main(){
	int n,quadrato;
	int potenza,parteDx,parteSx;
	int flag=0,cifre=0;
	scanf("%d",&n);
	
	if(n>0){
		quadrato=n*n;
		potenza=1;

		
		do{
		parteSx=quadrato/potenza;
		parteDx=quadrato%potenza;
		
		if(parteSx+parteDx==n)
			flag=1;
		else
			cifre++;
			
		potenza*=10;
		}while(parteSx!=0 && !flag);
		//AND perchè se non fosse di Kaprekar non uscirebbe mai dal ciclo
	} else 
		printf("errore\n");
		
	if(flag==1){
		printf("Si\n");
		printf("%d+%d\n",quadrato/(int)pow(10,cifre),quadrato%(int)pow(10,cifre));
	//pow castato ad in perché restituisce un double
	}
	else
		printf("No\n");
	return 0;
}
```
### Note
**Mai usare**:
- break; (se non per switch)
- continue;
- goto ...;
# Switch
## Definizione e Concetto

Lo switch (o selettore) è una struttura di controllo condizionale utilizzata per eseguire diversi blocchi di codice in base al valore di una singola espressione. Funziona come un'alternativa più pulita e leggibile a una serie di costrutti `if-else if-else` concatenati.
## Sintassi Base

```C
switch (espressione) {
    case valore1:
        // Codice eseguito se espressione == valore
        break;
    case valore2: 
        // Codice eseguito se espressione == valore2
        break;
    default:
        // Codice eseguito se nessun case corrisponde
        break;
}
```
## Caratteristiche Principali

• Espressione Selettrice: Solitamente deve valutare un tipo intero, carattere (`char`) o enumerazione (`enum`).
• Istruzione `break`: Interrompe l'esecuzione dello `switch` ed esce dal blocco. Senza `break`, l'esecuzione "decade" nei casi successivi (fall-through).
• Clausola `default`: Opzionale; viene eseguita quando nessun `case` corrisponde al valore dell'espressione.