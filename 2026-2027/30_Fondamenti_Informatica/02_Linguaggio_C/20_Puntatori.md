---
tags:
  - tipi-di-dato
  - puntatori
  - indirizzi-di-memoria
date: 2026-11-05
materia:
fonte:
---
# Puntatori
Ogni dato è assegnato ad un indirizzo di memoria.
Il puntatore è una *variabile che ospita un indirizzo di memoria*

- & operatore di referenziazione (associa alla variabie l'indirizzo)
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
## Operazione di dereferenziazione
puntatore -> (operatore di dereferenziazione) puntatore -> valore
``` C
printf("%f\n", *ptn); //scrive il valore alla variabile a cui punta ptr
```

> [!important] Tipizzazione dei puntatori
> I puntatori sono tipizzati perché diversamente non potrebbe funzionare la dereferenziazione


## Note collegate
- [[00_MOC_FdI]]
- [[05_Tipi_di_Dato]]
- [[FunzioniC.png]]

#materia/argomento/sottoargomento
