---
tags:
  - FI
  - programmazione-c
  - sizeof
  - limits
  - float
date: 2026-09-24
materia: Fondamenti di Informatica
fonte: Linguaggio C
---

# sizeOf e librerie dei limiti

## sizeOf

`sizeof(int)` → # byte occupati da una variabile di tipo `int`

## Librerie

`<limits.h>`
- `INT_MAX` → max valore rappresentabile con `int`
- `INT_MIN`
- `UINT_MAX`
- `UINT_MIN`

`<float.h>`
- `FLT_MAX`
- `FLT_MIN`
- `FLT_EPSILON`
- `DBL_MAX`
- `DBL_MIN`
- `DBL_EPSILON`

## Note collegate
- [[00_MOC_FdI]]
- Precedente: [[06_Tipi_Semplici_Int_Char_Float_Double]]
- Successiva: [[08_Conversione_fra_Tipi]]

#FdI/c/sizeof-librerie
