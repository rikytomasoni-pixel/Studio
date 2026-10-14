---
created: 2026-09-16
materia: A1
tags:
  - materia/a1
  - tipo/nota-atomica
  - fonte/handwritten
  - lezione/2
  - argomento/numeri_reali
aliases: []
---
[[00_A1_Numeri_Reali|⬅️ Torna a Numeri Reali]]

# Campi Ordinati

Un insieme $\mathbb{K}$ con due operazioni $+$ e $\cdot$ è un **campo** se valgono:

**Somma**
- **S1** (commutativa): $a+b=b+a$
- **S2** (associativa): $(a+b)+c=a+(b+c)$
- **S3** (elemento neutro): $\exists\, 0$ tale che $a+0=a$
- **S4** (opposto): $\forall a\ \exists (-a)$ tale che $a+(-a)=0$

**Prodotto**
- **P1** (commutativa): $a\cdot b=b\cdot a$
- **P2** (associativa): $(ab)c=a(bc)$
- **P3** (elemento neutro): $\exists\, 1\neq 0$ tale che $a\cdot 1=a$
- **P4** (inverso): $\forall a\neq 0\ \exists a^{-1}$ tale che $a\cdot a^{-1}=1$

**Distributività** (**SP**): $a(b+c)=ab+ac$

Esempi: $\mathbb{R}$, $\mathbb{Q}$, $\mathbb{C}$ sono campi; $\mathbb{N}$ e $\mathbb{Z}$ **non** lo sono (mancano opposto e/o inverso). Vedi anche [[2026-09-14 A1 Lezione 1|gli insiemi numerici]].

## 2. Ordine totale e campo ordinato

Una relazione $\le$ è un **ordine totale** (cfr. [[2026-09-17 GAL Lezione 1|relazioni d'ordine]]) se:
- **O1** riflessiva: $a\le a$
- **O2** antisimmetrica: $a\le b \wedge b\le a \Rightarrow a=b$
- **O3** transitiva: $a\le b \wedge b\le c \Rightarrow a\le c$
- **O4** totale: $\forall a,b$ vale $a\le b$ oppure $b\le a$

Un campo è **ordinato** se in più valgono le compatibilità:
- **SO**: $a\le b \Rightarrow a+c\le b+c$
- **PO**: $c>0,\ a\le b \Rightarrow ac\le bc$

$\mathbb{R}$ e $\mathbb{Q}$ sono campi ordinati. $\mathbb{C}$ **non** lo è: l'equazione $z^2+1=0$ ha soluzioni $\pm i$, mentre in un campo ordinato $a^2+1>0$ sempre.

### Regole deducibili dagli assiomi
- $a\cdot 0=0$
- $-a=(-1)\,a$
- $1>0$
- $a^2\ge 0$ per ogni $a$
- $a^2+1\ge 1>0$, quindi $a^2+1\neq 0$ in ogni campo ordinato

---
Successivo: [[Maggioranti, Minoranti ed Estremi]]
