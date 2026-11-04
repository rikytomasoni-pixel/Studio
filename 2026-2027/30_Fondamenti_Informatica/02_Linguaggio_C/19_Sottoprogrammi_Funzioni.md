---
tags:
  - funzioni
  - FI
  - input-output
  - struttura-programma
date: 2026-11-04
materia: Fondamenti di Informatica
fonte:
---
![[FunzioniC.png]]

1. Riuso
2. Modificabilità
3. Astrazione
4. Strutturazione
# Sottoprogrammi e Funzioni
## Prototipo

*tipo output* **nome funzione**(*tipo input*);
Gli input verranno chiamati **parametri formali** gli output **valori di ritorno**

``` C
int factorial(int);
```
### Parametri Formali
- zero o pù
- di ogni tipo (primitivi, user-defined, scalari, composti)
### Valore di ritorno
- al più 1 valore di ritotno
- scalare (primitivo, user-defined), Struct [NO ARRAY]
- opzione ```void```
## Definizione

Si da il nome ai parametri formali e si *dichiarano variabili locali* nel *corpo della funzione*
``` C
int factorial(int n){
	int fatt, i;
	fatt = 1;
	for(i = 2; i <= n; i++)
		fatt *= i;
		
	return fatt;
}
```

## Invocazione/Chiamata

Si da in pasto alla funzione i **parametri attuali** che devono avere una corrispondenza con i formali
```C
fatt = factorial(num);
```
## Note collegate
- [[05_Tipi_di_Dato]]
- [[03_Struttura_di_un_Programma_C]]
- [[04_Input_Output_e_Stream]]
- [[19_Funzioni_Generalità]]