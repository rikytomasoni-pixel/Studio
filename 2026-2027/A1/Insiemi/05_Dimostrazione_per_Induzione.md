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

Si usa per dimostrare la verità di un'implicazione universale della forma $\forall m \in \mathbb{N},\ P(m)$ vera. Si articola in due passi:

1. si dimostra che $P(0)$ è vera ($m=0$);
2. si dimostra che **se** $P(m)$ è vera **allora** è vera anche $P(m+1)$, cioè $\forall m \in \mathbb{N},\ P(m) \Rightarrow P(m+1)$.

$P(m)$ prende il nome di **ipotesi di induzione**.

Informalmente: $P(0) \text{ vera} \xrightarrow{i} P(1) \text{ vera} \xrightarrow{ii} P(2) \text{ vera} \xrightarrow{iii} \dots$

> [!theorem] Disuguaglianza di Bernoulli
> $\forall m \in \mathbb{N},\ \forall x \in \mathbb{R}$ con $x > -1$:
> $$(1+x)^m \geq 1+mx$$

**Dimostrazione (per induzione).** Sia $P(m)$: $\forall x \in \mathbb{R}$ con $x>-1$, $(1+x)^m \geq 1+mx$.

**i) Verifichiamo $P(0)$ vera**

$$(1+x)^0 \geq 1+0\cdot x \;\Longleftrightarrow\; 1 \geq 1 \quad \text{vera}$$

**ii) Verifichiamo $P(m) \Rightarrow P(m+1)$ vera $\forall m \in \mathbb{N}$**

$$P(m+1): \quad (1+x)^{m+1} \geq 1+(m+1)x$$

Assumendo $P(m)$ vera, partiamo da:

$$(1+x)^{m+1} = (1+x)^m (1+x)$$

dove $(1+x)>0$ e $(1+x)^m \geq 1+mx$ per ipotesi di induzione $P(m)$. Quindi:

$$(1+x)^{m+1} = (1+x)^m(1+x) \geq (1+mx)(1+x) = 1+mx+x+mx^2 = 1+(m+1)x+\underbrace{mx^2}_{\geq 0}$$

da cui $1+(m+1)x+mx^2 \geq 1+(m+1)x$, quindi:

$$(1+x)^{m+1} \geq (1+mx)(1+x) \geq 1+(m+1)x$$

cioè $P(m+1)$ è vera. Pertanto $P(m) \Rightarrow P(m+1)$ è vera $\forall m \in \mathbb{N}$, e per induzione $P(m)$ è vera $\forall m \in \mathbb{N}$. $\blacksquare$

### Note collegate
- [[00_MOC_A1]]
- [[03_Dimostrazioni]] — altri metodi di dimostrazione
- [[04_Dimostrazione_per_Assurdo]]
- [[02_Logica]] — implicazione universale
- [[01_Insiemi_Numerici]] — l'insieme $\mathbb{N}$