---
tags:
  - FI
  - programmazione-c
  - tipi-di-dato
  - int
  - char
  - float
  - double
date: 2026-09-24
materia: Fondamenti di Informatica
fonte: Linguaggio C
---

# Dati predefiniti semplici

## INT → numeri interi con segno

- Complemento a 2
- tipicamente 32 bit (4 byte)
- $[-2^{31},\ 2^{31}-1]$
- operazioni aritmetiche: `+`, `*`, `-`, `/`, `%`
- Lettura-scrittura `%d`
- Varianti:
	- `unsigned int` → `unsigned int y;` → `%u` → binario naturale
	- `short`, `long` → numeri interi con segno, tipicamente 16 bit / 64 bit

## CHAR → caratteri

- 8 bit (1 byte) → $[0,\ 255]$
- codifica ASCII
- `%c`
- operazioni

## FLOAT → numeri razionali

- virgola mobile in singola precisione
- IEEE 754 → 32 bit
- operazioni NO `%`

## DOUBLE → numeri razionali

- virgola mobile in doppia precisione
- IEEE 754 → 64 bit
- `scanf` → `%lf`
- `printf` → `%f`

## Note collegate
- [[00_MOC_FdI]]
- Precedente: [[05_Tipi_di_Dato]]
- Successiva: [[07_sizeof_e_Librerie_limits_float]]

#FdI/c/tipi-semplici
