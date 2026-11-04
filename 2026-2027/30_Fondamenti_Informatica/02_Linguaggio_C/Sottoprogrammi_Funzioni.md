![[FunzioniC.png]]

1. Riuso
2. Modificabilità
3. Astrazione
4. Strutturazione
# Prototipo

*tipo output* **nome funzione**(*tipo input*);
Gli input verranno chiamati parametri gli output valori di ritorno

``` C
int factorial(int);
```
# Definizione

Si assegnano *variabili locali* e il *corpo della funzione*
``` C
int factorial(int n){
	int fatt, i;
	fatt = 1;
	for(i = 2; i <= n; i++)
		fatt *= i;
		
	return fatt;
}
```

# Invocazione/Chiamata
```C
fatt = factorial()
```