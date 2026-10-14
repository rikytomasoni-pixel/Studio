---
created: 2026-10-02
materia: A1
tags:
  - stato/da-revisionare
  - materia/a1
  - tipo/nota-atomica
  - fonte/handwritten
  - lezione/7
  - argomento/successioni_e_limiti
aliases: []
origine: UpdateVault
---
[[00_A1_Successioni_e_Limiti|⬅️ Torna a Successioni e Limiti]]

# Gerarchia degli Infiniti

> [!abstract] Teorema — Gerarchia degli infiniti
> Per $n\to\infty$, valgono i seguenti confronti (dal più "lento" al più "veloce" a divergere):
> 1. $\displaystyle\lim_{n\to\infty} \dfrac{(\log n)^\alpha}{n^\beta} = 0 \qquad \forall\, \alpha,\beta>0$
> 2. $\displaystyle\lim_{n\to\infty} \dfrac{n^\alpha}{q^n} = 0 \qquad \forall\, \alpha>0,\ q>1$
> 3. $\displaystyle\lim_{n\to\infty} \dfrac{q^n}{n!} = 0 \qquad \forall\, q\in\mathbb{R}$
> 4. $\displaystyle\lim_{n\to\infty} \dfrac{n!}{n^n} = 0$

Informalmente, per $n\to\infty$:
$$\log n \ll n^\alpha \ll q^n\ (q>1) \ll n! \ll n^n$$

## Applicazione: esempio di uso nella gerarchia

**Esempio.** $a_n = \dfrac{n}{n!}$

$$\lim_{n\to\infty} \dfrac{n}{n!} = 0 \qquad \text{per gerarchia degli infiniti}$$

---
Precedente: [[Teoremi del Confronto]]
