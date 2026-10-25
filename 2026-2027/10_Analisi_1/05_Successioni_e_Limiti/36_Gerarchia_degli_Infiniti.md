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
> $$(\log_a n)^\beta \;\ll\; n^\alpha \;\ll\; a^n \;\ll\; n! \;\ll\; n^n \qquad \forall\, \beta>0,\ \forall\, \alpha>0,\ \forall\, a>1$$
> cioè
> 1. $\displaystyle\lim_{n\to\infty} \dfrac{(\log_a n)^\beta}{n^\alpha} = 0$
> 2. $\displaystyle\lim_{n\to\infty} \dfrac{n^\alpha}{a^n} = 0$
> 3. $\displaystyle\lim_{n\to\infty} \dfrac{a^n}{n!} = 0$
> 4. $\displaystyle\lim_{n\to\infty} \dfrac{n!}{n^n} = 0$

**Osservazione.** Il punto 4 segue da $\displaystyle\lim_{n\to\infty} \dfrac{n^n}{n!} = +\infty$ (vedi [[39_Criterio_del_Rapporto]]):
$$\lim_{n\to\infty} \dfrac{n!}{n^n} = \lim_{n\to\infty} \left(\dfrac{n^n}{n!}\right)^{-1} = 0$$

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
