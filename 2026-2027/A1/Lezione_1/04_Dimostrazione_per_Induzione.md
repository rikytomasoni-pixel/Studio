---
tags:
  - AM1
  - dimostrazioni
  - induzione
  - disuguaglianza-di-bernoulli
data: 2026-09-14
fonte: Lezione 1
---

# Dimostrazione per induzione

Si usa per dimostrare la verità di un'implicazione universale della forma $\forall n \in \mathbb{N},\ P(n)$ vera. Si articola in due passi:

1. si dimostra che $P(0)$ è vera ($n=0$);
2. si dimostra che **se** $P(n)$ è vera **allora** è vera anche $P(n+1)$, cioè $\forall n \in \mathbb{N},\ P(n) \Rightarrow P(n+1)$.

$P(n)$ prende il nome di **ipotesi di induzione**.

Informalmente: $P(0) \text{ vera (i)} \Rightarrow P(1) \text{ vera (ii)} \Rightarrow P(2) \text{ vera (ii)} \Rightarrow \dots$

> [!theorem] Disuguaglianza di Bernoulli
> $\forall n \in \mathbb{N},\ \forall x \in \mathbb{R}$ con $x > -1$:
> $$(1+x)^n \geq 1+nx$$

**Dimostrazione (per induzione).** Sia $P(n)$: $\forall x \in \mathbb{R}$ con $x>-1$, $(1+x)^n \geq 1+nx$.

**i) Verifichiamo $P(0)$ vera**

$$(1+x)^0 \geq 1+0\cdot x \;\Longleftrightarrow\; 1 \geq 1 \quad \text{vera}$$

**ii) Verifichiamo $P(n) \Rightarrow P(n+1)$ vera $\forall n \in \mathbb{N}$**

$$P(n+1): \quad (1+x)^{n+1} \geq 1+(n+1)x$$

Assumendo $P(n)$ vera, partiamo da:

$$(1+x)^{n+1} = (1+x)^n (1+x)$$

dove $(1+x)>0$ e $(1+x)^n \geq 1+nx$ per ipotesi di induzione $P(n)$. Quindi:

$$(1+x)^{n+1} = (1+x)^n(1+x) \geq (1+nx)(1+x) = 1+nx+x+nx^2 = 1+(n+1)x+\underbrace{nx^2}_{\geq 0}$$

da cui $1+(n+1)x+nx^2 \geq 1+(n+1)x$, quindi:

$$(1+x)^{n+1} \geq (1+nx)(1+x) \geq 1+(n+1)x$$

cioè $P(n+1)$ è vera. Pertanto $P(n) \Rightarrow P(n+1)$ è vera $\forall n \in \mathbb{N}$, e per induzione $P(n)$ è vera $\forall n \in \mathbb{N}$. $\blacksquare$

### Note collegate
- [[00_MOC_A1]]
- [[02_Dimostrazioni]] — altri metodi di dimostrazione
- [[03_Dimostrazione_per_Assurdo]]
- [[01_Logica]] — implicazione universale
- [[00_Insiemi_Numerici]] — l'insieme $\mathbb{N}$