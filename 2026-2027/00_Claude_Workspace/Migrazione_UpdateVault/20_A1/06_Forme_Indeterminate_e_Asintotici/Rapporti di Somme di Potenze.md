---
created: 2026-10-07
materia: A1
tags:
  - stato/da-revisionare
  - materia/a1
  - tipo/nota-atomica
  - fonte/handwritten
  - lezione/8
  - argomento/forme_indeterminate_e_asintotici
aliases: []
origine: UpdateVault
---
[[00_A1_Forme_Indeterminate_e_Asintotici|⬅️ Torna a Forme Indeterminate e Asintotici]]

# Rapporti di Somme di Potenze

## Esempi con limiti di successioni razionali (rapporto di polinomi/potenze e funzioni limitate)

**Esempio.**
$$a_n = \dfrac{n+\sin n + \log\log n}{2n+\cdots}$$
$$\lim_{n\to\infty} a_n = 0$$

**Osservazione.** $a_n = \dfrac{P}{Q}$, dove $P, Q$ sono somme di potenze di $n$ e di funzioni limitate in $n$ (o "trascurabili" rispetto a potenze di $n$): se la potenza massima di $n$ in $P$ (positiva) è più piccola della potenza massima di $n$ in $Q$ (positiva), allora, ragionando come sopra,
$$\lim_{n\to\infty} a_n = 0$$

**Esempio.**
$$a_n = \dfrac{5n+\cdots}{n+\cdots} \quad\Rightarrow\quad \lim_{n\to\infty} a_n = \dfrac{5+0}{1+0} = 5$$

**Osservazione.** $a_n=\dfrac{P}{Q}$, dove $P,Q$ sono somme di potenze di $n$ e di funzioni limitate (o trascurabili rispetto a potenze di $n$), dove la potenza massima di $n$ in $P$ è uguale alla potenza massima di $n$ in $Q$ (entrambe positive). Allora
$$\lim_{n\to\infty} a_n = l$$
dove $l$ è il quoziente del coefficiente della potenza massima di $n$ in $P$ e del coefficiente della potenza massima di $n$ in $Q$.

**Esempio.**
$$a_n = \dfrac{\sin n + \log\log n + \cdots}{\log n + \cdots}$$
$$\lim_{n\to\infty} a_n = -\infty$$

**Osservazione.** $a_n=\dfrac{P}{Q}$, dove $P,Q$ sono somme di potenze di $n$ e di funzioni limitate di $n$ (o trascurabili rispetto a potenze di $n$), dove la potenza massima di $n$ in $P$ (positiva) è maggiore della potenza massima di $n$ in $Q$ (positiva). Allora
$$a_n \to \pm\infty, \quad \text{segno deciso dal prodotto dei segni dei coefficienti delle potenze massime di } n \text{ in } P, Q$$

**Esempio.** $a_n = \dfrac{n!}{n^n} \to 0$ per gerarchia degli infiniti (vedi [[Gerarchia degli Infiniti]]).

---
Successivo: [[Aritmetizzazione dell'Infinito e Forme di Indeterminazione]]
