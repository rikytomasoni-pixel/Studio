---
tags:
  - FI
  - programmazione-c
  - switch
date: 2026-09-24
materia: Fondamenti di Informatica
fonte: Linguaggio C
---

# Switch

## Definizione e Concetto

Lo switch (o selettore) è una struttura di controllo condizionale utilizzata per eseguire diversi blocchi di codice in base al valore di una singola espressione. Funziona come un'alternativa più pulita e leggibile a una serie di costrutti `if-else if-else` concatenati (vedi [[15_Condizione_if_else]]).

## Sintassi Base

```C
switch (espressione) {
    case valore1:
        // Codice eseguito se espressione == valore
        break;
    case valore2: 
        // Codice eseguito se espressione == valore2
        break;
    default:
        // Codice eseguito se nessun case corrisponde
        break;
}
```

## Caratteristiche Principali

- Espressione Selettrice: Solitamente deve valutare un tipo intero, carattere (`char`) o enumerazione (`enum`).
- Istruzione `break`: Interrompe l'esecuzione dello `switch` ed esce dal blocco. Senza `break`, l'esecuzione "decade" nei casi successivi (fall-through).
- Clausola `default`: Opzionale; viene eseguita quando nessun `case` corrisponde al valore dell'espressione.

## Note collegate
- [[00_MOC_FdI]]
- Precedente: [[17_Numeri_di_Kaprekar]]

#FdI/c/switch
