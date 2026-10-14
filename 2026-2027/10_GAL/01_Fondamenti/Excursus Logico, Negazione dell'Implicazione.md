---
created: 2026-09-17
materia: GAL
tags:
  - materia/gal
  - tipo/nota-atomica
  - fonte/handwritten
  - lezione/1
  - argomento/fondamenti
aliases: []
---
[[00_GAL_Fondamenti|⬅️ Torna a Fondamenti]]

# Excursus Logico, Negazione dell'Implicazione

«condizione 1» $\Rightarrow$ «condizione 2» equivale a «negazione di condizione 2» $\Rightarrow$ «negazione di condizione 1» (contronominale).

*Esempio*: «vado in bici in solito» $\Rightarrow$ «frequenza cardiaca aumenta» equivale a «frequenza cardiaca non aumenta» $\Rightarrow$ «non sono andato in bici in solito».

Applicando la contronominale:

$$
\#F \neq \#A \implies F \subseteq A \times B \text{ NON è una funzione}
$$

**Attenzione!** Il fatto che il numero di elementi di $F$ e $A$ sia lo stesso non garantisce che io abbia una funzione. Ci sono relazioni $F \subseteq A \times B$ con $\#F = \#A$ che non sono funzioni.

*Esempio*: $A = \{\text{anguria, banana, lampone, limone}\}$, $B = \{\text{"a"},\text{"b"},\text{"l"}\}$, $\#A = 4$. La relazione $\{(\text{anguria},\text{"a"}),(\text{banana},\text{"b"}),(\text{lampone},\text{"l"}),(\text{anguria},\text{"b"})\}$ ha $\#F = 4$ ma **non è una funzione** (anguria ha due immagini e limone nessuna).

---
Precedente: [[Funzioni]] · Successivo: [[Iniettività Surgettività Biettività]]
