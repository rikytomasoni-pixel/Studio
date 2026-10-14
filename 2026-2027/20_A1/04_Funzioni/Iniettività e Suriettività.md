---
created: 2026-09-25
materia: A1
tags:
  - stato/da-revisionare
  - materia/a1
  - tipo/nota-atomica
  - fonte/handwritten
  - lezione/5
  - argomento/funzioni
aliases: []
origine: UpdateVault
---
[[00_A1_Funzioni|⬅️ Torna a Funzioni]]

# Iniettività e Suriettività

> [!info] Definizione
> Data $f:A\to B$:
> - se $\operatorname{Im}f=B$, $f$ si dice **suriettiva**
> - $f$ si dice **iniettiva** se (equivalentemente):
>   1. $\forall\, x_1,x_2\in A$: $\ x_1\neq x_2 \ \Rightarrow\ f(x_1)\neq f(x_2)$
>   2. $\forall\, x_1,x_2\in A$: $\ f(x_1)=f(x_2) \ \Rightarrow\ x_1=x_2$
>   3. $\forall\, y\in\operatorname{Im}f\ \ \exists!\, x\in A: \ f(x)=y$

**Osservazione.** Sull'equazione $f(x)=y$: se $y\in\operatorname{Im}f$ esiste $x\in\mathcal{D}(f)$ tale che $f(x)=y$, per definizione di $\operatorname{Im}f$.

Allora, se $f$ **suriettiva**, $f(x)=y$ ammette sempre **almeno** una soluzione $x\in\mathcal{D}(f)$, $\forall\, y\in B$.

Se $f$ **iniettiva**, $f(x)=y$ può non avere soluzioni $x\in\mathcal{D}(f)$ per qualche $y\in B$, ma se ne esiste una ($\Leftrightarrow y\in\operatorname{Im}f$) essa è **unica**. Quindi l'equazione ammette **al più** una soluzione, $\forall\, y\in B$.

---
Precedente: [[Composizione di Funzioni]] · Successivo: [[Funzione Inversa]]
