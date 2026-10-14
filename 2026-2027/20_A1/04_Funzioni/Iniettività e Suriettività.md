---
created: 2026-09-25
materia: A1
tags:
  - materia/a1
  - tipo/nota-atomica
  - fonte/handwritten
  - lezione/5
  - argomento/funzioni
aliases: []
---
[[00_A1_Funzioni|⬅️ Torna a Funzioni]]

# Iniettività e Suriettività

Data $f:A\to B$ (cfr. [[2026-09-17 GAL Lezione 1|funzioni iniettive e suriettive]]):

- $f$ è **suriettiva** se $\operatorname{Im}f=B$;
- $f$ è **iniettiva** se (equivalentemente):
  1. $\forall x_1,x_2\in A$: $x_1\neq x_2\Rightarrow f(x_1)\neq f(x_2)$;
  2. $\forall x_1,x_2\in A$: $f(x_1)=f(x_2)\Rightarrow x_1=x_2$;
  3. $\forall y\in\operatorname{Im}f\ \ \exists!\,x\in A:\ f(x)=y$.

### Lettura sull'equazione $f(x)=y$
- Se $y\in\operatorname{Im}f$ esiste $x\in\mathcal{D}(f)$ con $f(x)=y$ per definizione di $\operatorname{Im}f$. Quindi se $f$ è **suriettiva**, $f(x)=y$ ammette **almeno una** soluzione $\forall y\in B$.
- Se $f$ è **iniettiva**, $f(x)=y$ può non avere soluzioni per qualche $y\in B$, ma se ne esiste una ($\iff y\in\operatorname{Im}f$) essa è **unica**. L'equazione ammette quindi **al più una** soluzione $\forall y\in B$.

---
Precedente: [[Composizione di Funzioni]] · Successivo: [[Funzione Inversa]]
