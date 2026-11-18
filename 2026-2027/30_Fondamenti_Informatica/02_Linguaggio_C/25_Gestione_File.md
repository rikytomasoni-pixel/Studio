---
tags:
  - FdI/c
  - File
date: 2026-11-18
materia: Fondamenti di Informatica
fonte: Linguaggio C
---
# Gestione File

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
*descrittore* =  **fopen**(*pathname*, *modalità d'accesso*);

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
**fscanf**(*identificatore*, ...);
Funzione che restituisce:
-  # 
- Costante **EOF** "end of file" = -1
```C
fscanf(fp, ...);
```
### Lettura
```C
while(fscanf(f))
```
## Chiusura del file
```C
fclose(fp);
```
## Note collegate
- [[00_MOC_Materia]]

#materia/argomento/sottoargomento
