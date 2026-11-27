---
tags:
  - FI
  - programmazione-c
  - cicli
  - esercizio
  - kaprekar
date: 2026-09-24
materia: Fondamenti di Informatica
fonte: Linguaggio C
---

# Excursus sui numeri di Kaprekar

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
	//pow castato ad int perché restituisce un double
	}
	else
		printf("No\n");
	return 0;
}
```

## Note collegate
- [[00_MOC_FdI]]
- Precedente: [[16_Cicli_Iterativi]]
- Successiva: [[18_Switch]]

#FdI/c/esercizi/kaprekar
