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
> 1. $\displaystyle\lim_{n\to\infty}\dfrac{\log_a n}{n^\alpha}=0 \qquad \forall\,\alpha>0,\ \forall\,a>1$
> 2. $\displaystyle\lim_{n\to\infty}\dfrac{n^\alpha}{a^n}=0 \qquad \forall\,\alpha>0,\ \forall\,a>1$
> 3. $\displaystyle\lim_{n\to\infty}\dfrac{a^n}{n!}=0 \qquad \forall\,a>1$
> 4. $\displaystyle\lim_{n\to\infty}\dfrac{n!}{n^n}=0$

Nella Lezione 8 la gerarchia è riassunta in un riquadro:
$$(\log_a n)^\beta\ \ll\ n^\alpha\ \ll\ a^n\ \ll\ n!\ \ll\ n^n \qquad \forall\,\beta>0,\ \forall\,\alpha>0,\ \forall\,a>1$$

**Esempio.** $\displaystyle\lim_{n\to\infty}n^{1/n}=1$ (forma $[\infty^0]$): si usa la gerarchia degli infiniti, vedi [[02_Criterio_del_Rapporto]].

> [!warning] Differenze rispetto alla trascrizione precedente
> Rispetto al PDF manoscritto la versione precedente di questa nota aveva: $(\log n)^\alpha/n^\beta$ con $\alpha,\beta>0$ (vero, ma nel PDF c'è $\log_a n/n^\alpha$ e, nella L8, $(\log_a n)^\beta$); $a^n/n!\to0$ per ogni $q\in\mathbb{R}$ (vero, ma il PDF scrive $a>1$); e l'esempio $\frac{n}{n!}\to0$, che **non compare nel PDF**. Se vuoi tenerli, sono tutti enunciati corretti.

### Note collegate
- [[00_MOC_A1]]
- [[03_Teoremi_del_Confronto]]
- [[00_Successione_Convergente_e_Limitata]] — esempio progressione geometrica $q^n$
- [[02_Limiti_di_Successioni]]
- [[02_Criterio_del_Rapporto]] — usa la gerarchia degli infiniti negli esempi
- [[03_Confronti_Asintotici]] — ordine di infinito tra successioni
