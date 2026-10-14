---
tags:
  - AM1
  - successioni
  - gerarchia-degli-infiniti
  - limiti
data: 2026-10-02 e 2026-10-07
fonte: Lezione 7 e Lezione 8
---

# Gerarchia degli infiniti

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

### Note collegate
- [[00_MOC_Analisi_1]]
- [[35_Teoremi_del_Confronto]]
- [[32_Successione_Convergente_e_Limitata]] — esempio progressione geometrica $q^n$
- [[30_Limiti_di_Successioni]]
- [[39_Criterio_del_Rapporto]] — usa la gerarchia degli infiniti negli esempi
- [[40_Confronti_Asintotici]] — ordine di infinito tra successioni

#AM1/successioni-e-limiti/gerarchia-degli-infiniti
