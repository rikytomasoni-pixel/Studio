![[FunzioniC.png]]

1. Riuso
2. Modificabilità
3. Astrazione
4. Strutturazione
# Prototipo

*tipo output* **nome funzione**(*tipo input*);
Gli input verranno chiamati parametri formali gli output valori di ritorno

``` C
int factorial(int);
```
# Definizione

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

# Invocazione/Chiamata

Si da in pasto alla funzione i parametri attuali che devono avere una corrispondenza con i formal
```C
fatt = factorial(num);
```