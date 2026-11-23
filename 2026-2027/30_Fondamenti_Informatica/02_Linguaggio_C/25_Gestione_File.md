---
tags:
  - FI
  - programmazione-c
  - file
  - fopen
  - fprintf
  - fscanf
  - file-binari
  - memoria
date: 2026-11-18
materia: Fondamenti di Informatica
fonte: Linguaggio C
---
# Gestione File

*Lettura e scrittura su memoria di massa con la libreria `stdio.h`: file di testo e file binari.*
## Cenni sulla memoria

| Memoria di Massa    | Memoria Centrale         |
| ------------------- | ------------------------ |
| Lenta               | Veloce                   |
| Persistente         | Volatile                 |
| Capiente            | Poco Capiente            |
| Accesso Sequenziale | Accesso Diretto (random) |
## Puntatore al Descrittore del File
```C
FILE *fp; //apre il flusso di comunicazione
```
## Apertura del File
*file pointer* =  **fopen**(*pathname*, *modalità d'accesso*);

```C
fp = fopen("input.txt", "w"); 
```
### Tipi di File
- File di Testo (.txt)
	- sequenza di caratteri
- File binario (.bin)
	- sequenza di byte
### Modalità d'accesso
*per i file di testo*
- **`"r"` (Read):** Apre un file in sola lettura. Il file **deve esistere**, altrimenti `fopen()` restituisce `NULL`. Il cursore parte dall'inizio.
- **`"w"` (Write):** Apre un file in sola scrittura. Se il file esiste già, **il suo contenuto viene cancellato**; se non esiste, viene creato. Il cursore parte dall'inizio.
- **`"a"` (Append):** Apre un file in scrittura in coda. Mantiene i dati esistenti e aggiunge i nuovi alla fine. Se il file non esiste, viene creato.
- **`"r+"`:** Apre un file esistente sia in lettura che in scrittura. Non cancella il contenuto. Se il file non esiste, restituisce `NULL`.
- **`"w+"`:** Crea un nuovo file vuoto per lettura e scrittura. Se il file esiste già, **ne cancella tutto il contenuto**.
- **`"a+"`:** Apre un file per lettura e aggiunta in coda. Se non esiste, viene creato. La lettura può avvenire ovunque, ma **la scrittura avviene sempre alla fine**.
### Corretta esecuzione di fopen
```C
if(!fp){
	printf("Error.\n");
	return -1;
}
```

## Scrittura File di testo
**fprintf**(*descrittore*, ...);
```C
for(int i = 0; i <= 10; i++)
fprintf(fp, "%d\n", i);
```

**NB**
```C
//scrivere
fprintf(stdout, "...");
//equivale a
printf("...");
```
## Lettura File di Testo
**fscanf**(*file pointer*, ...);
Funzione che restituisce:
- il numero di elementi effettivamente letti (1 se il carattere di formattazione corrisponde, 0 altrimenti)
- la costante **EOF** "end of file" = -1 se non legge nulla perché il file è finito
```C
fscanf(fp, ...);
```
**fgets**(*stringa*, *dimensione*, *file pointer*);
Funzione che legge i primi DIM-1 caratteri e si ferma prima se incontra il carattere '**\n**'
### Lettura di caratteri
```C
while(fscanf(fp, "%d", &i) == 1)
	printf("%d\n", i);
```
### Lettura Stringhe
```C
while(fgets(str, DIM, fp) != NULL)
	printf("%s", str);
```

## File Binari
```C
FILE *fp;

fp = fopen("new_file.bin", "wb");
//qualsiasi metodo di accesso visto fino ad ora seguito da una 'b'
if(!fp){
	printf("Error\n");
	return -1;
} 
```
### Lettura e scrittura
```C
#define DIM 20
float array[DIM];
int n;
for(int i = 0; i < DIM; i++)
	array[i] = 1.0 / (1 + i);
```
- **fread**(*indirizzo di partenza, dimensione in byte di un elemento, # elementi , file pointer*)
```C
n = fread(array, sizeof(float), DIM/2, fp);
printf("Ho letto %d elementi.\n", n);
```
- **fwrite**(*indirizzo di partenza, dimensione in byte di un elemento, # elementi , file pointer*)
```C
fwrite(array, sizeof(float), DIM, fp);
```
### Altre funzioni
```C
int pos = ftell(fp); //restituisce la posizione corrente nel file (binario)
fseek(fp, offset, origin);//modifica la posizione di read/write nel file
/* 
SEEK_SET costante per l'inizio del file
fseek(fp, 5, SEEK_SET);

SEEK_END fine del file
SEEK_CUR posizione corrente
*/
```
## Chiusura del file
```C
fclose(fp);
```
## Note collegate
- [[00_MOC_FdI]]
- Precedente: [[24_Ricorsione]]
- [[04_Input_Output_e_Stream]] — `scanf`/`printf` su `stdin`/`stdout`: `fscanf`/`fprintf` sono la versione per file (`stdout` è un `FILE *`)
- [[10_Stringhe_in_C]] — `fgets` per leggere stringhe da file
- [[09_Array_Monodimensionali]] — `fread`/`fwrite` leggono e scrivono interi array
- [[14_Struct]] — `fwrite`/`fread` anche su struct
- [[20_Puntatori]] — `FILE *fp` è un puntatore al descrittore del file
- [[07_sizeof_e_Librerie_limits_float]] — `sizeof` come dimensione dell'elemento in `fread`/`fwrite`
- [[16_Cicli_Iterativi]] — cicli `while` di lettura fino a `EOF`
- Successiva: [[26_Allocazione_Dinamica_della_Memoria]]

#FdI/c/file
