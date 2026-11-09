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

- & **operatore di referenziazione** (associa alla variabile l'indirizzo)
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
`*` **operatore di dereferenziazione**: applicato a un puntatore restituisce il valore contenuto all'indirizzo a cui punta
``` C
printf("%f\n", *ptr); //scrive il valore alla variabile a cui punta ptr
```

> [!important] Tipizzazione dei puntatori
> I puntatori sono tipizzati perché diversamente non potrebbe funzionare la dereferenziazione


> [!WARNING] Puntatore a Void
> Il puntatore di tipo void non è tipizzato, ma non può essere dereferenziato se non tramite casting

## Passaggio per indirizzo
Similmente al passaggio per copia di [[19_Sottoprogrammi_Funzioni]]
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

## Puntatori ed Array
### Array come puntatori

L'array in C è un puntatore **costante** che punta al suo primo elemento e occupa le N celle di memoria successive, il fatto che sia costante implica che non possiamo cambiarne il valore in eseguzione

```C
int A[5], i;

for(i = 0; i < 5; i++)
	A[i] = 2 * i; 

//Scrivere &A[0] equivale a scrivere A, A punta al primo elemento dell'array
printf("%p\n", A);
printf("%p\n", &A[0]);

```

## Aritmetica dei Puntatori
### Unità di memoria

Quando si fanno operazioni con i puntatori l'operazione usa come unità di misura la dimensione del tipo del puntatore (int 4 byte, double 8 byte) per spostarsi nelle celle di memoria

``` C
int *ptr

ptr = &A[1]; //che è come scrivere il puntatore alla cella A+1

ptr = ptr + 2; //operazione in "unità di sizeOf(tipo)" il puntatore si sposta avanti di 2 byte

//in particolare scrivere &A[2] equivale a A + 2
//altrettanto scrivere *(A+2) equivale a A[2]

printf("%d\n", ptr - A); //la differenza è sempre in unità di memoria quindi è come se stessimo scrivendo #byte ptr - #byte A (= 3)
```


## Note collegate
- [[00_MOC_FdI]]
- [[05_Tipi_di_Dato]]
- [[19_Sottoprogrammi_Funzioni]]

#FdI/c/puntatori

