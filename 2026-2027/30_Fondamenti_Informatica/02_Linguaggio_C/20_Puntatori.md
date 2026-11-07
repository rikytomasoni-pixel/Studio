---
tags:
  - tipi-di-dato
  - puntatori
  - indirizzi-di-memoria
date: 2026-11-05
materia: Fondamenti di Informatica
fonte:
---
# Puntatori
Ogni dato è assegnato ad un indirizzo di memoria.
Il puntatore è una *variabile che ospita un indirizzo di memoria*

- & **operatore di referenziazione** (associa alla variabie l'indirizzo)
- %p carattere di formato

```C
float x = 3;
printf("%p\n",&x);
```

## Dichiarazione
``` C
<tipo> *<identificatore>
float *ptr;
ptr = &x //il puntatore punta all'indirizzo di x;
```

``` C
float *ptr1 = NULL; //dobbiamo ancora assegnare un indirizzo al puntatore
```

## Operazione di dereferenziazione
puntatore -> (operatore di dereferenziazione) puntatore -> valore
``` C
printf("%f\n", *ptn); //scrive il valore alla variabile a cui punta ptr
```

> [!important] Tipizzazione dei puntatori
> I puntatori sono tipizzati perché diversamente non potrebbe funzionare la dereferenziazione


> [!WARNING] Puntatore a Void
> Il puntatore di tipo void non è tipizzato, ma non può essere dereferenziato se non tramite casting

## Passaggio per indirizzo
Similmente al passaggio per copia di [[FunzioniC.png]]
```C
void swap(int *x, int *y){ //puntatori come parametri formali
	int temp;
	temp = *x;
	*x = *y;
	*y = temp;
}
int main(){
	int a, b;
	scanf("%d%d",&a,&b);
	swap(&a,&b);//parametri attuali come indirizzi
	printf("%d, %d\n",a,b);
	return 0;
}
```
## Note collegate
- [[00_MOC_FdI]]
- [[05_Tipi_di_Dato]]
- [[FunzioniC.png]]

#FdI/c/puntatori

