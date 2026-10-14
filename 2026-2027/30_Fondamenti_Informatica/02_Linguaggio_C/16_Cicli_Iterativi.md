---
tags:
  - FI
  - programmazione-c
  - cicli
  - while
  - for
date: 2026-09-24
materia: Fondamenti di Informatica
fonte: Linguaggio C
---

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

Esempio di applicazione: [[17_Numeri_di_Kaprekar]]

## Note

**Mai usare**:
- break; (se non per switch)
- continue;
- goto ...;

Vedi [[18_Switch]].

## Note collegate
- [[00_MOC_FdI]]
- Precedente: [[15_Condizione_if_else]]
- Successiva: [[17_Numeri_di_Kaprekar]]

#FdI/c/cicli
