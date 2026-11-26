---
tags:
  - AM1
  - derivate
  - de-l-hopital
  - esempio
  - limiti-di-funzioni
data: 2026-11-18
lezione: 19
fonte: "AM1 L19 26-27.pdf (pag. 17-18)"
---

# Esempi di applicazione di de l'Hôpital

Si usa [[152_Teorema_di_de_l_Hopital]].

## Esempio 1: $\displaystyle\lim_{x\to0}\frac{(\sin x)^{42}}{x^{42}}$
$$\lim_{x\to0}\frac{(\sin x)^{42}}{x^{42}}=\lim_{x\to0}\frac{42(\sin x)^{41}\cos x}{42\,x^{41}}=\dots=1$$
(servono **42 volte** de l'Hôpital).

In alternativa, con il limite notevole ([[108_Limiti_Notevoli_di_Funzioni]]):
$$\lim_{x\to0}\frac{(\sin x)^{42}}{x^{42}}=\lim_{x\to0}\left(\frac{\sin x}{x}\right)^{42}=1^{42}=1$$

> [!tip] Quando conviene
> Spesso un limite notevole o un asintotico ([[106_Asintotico_e_o_piccolo_per_Funzioni]]) è molto più rapido di applicare de l'Hôpital ripetutamente.

## Esempio 2: $\displaystyle\lim_{x\to+\infty}\frac{x}{e^{\beta x}}=0\qquad\forall\beta>0$
$$\lim_{x\to+\infty}\frac{x}{e^{\beta x}}\overset{H}{=}\lim_{x\to+\infty}\frac{1}{\beta e^{\beta x}}=0$$
(l'ultimo passaggio per algebra dei limiti).

Questo esempio è il primo mattone per la [[155_Dimostrazione_della_Gerarchia_degli_Infiniti_con_de_l_Hopital|dimostrazione della gerarchia degli infiniti]].

## Note collegate
- [[176_Esempio_Limite_con_Sviluppi_di_Taylor]]
- [[152_Teorema_di_de_l_Hopital]]
- [[153_Controesempio_de_l_Hopital_Limite_delle_Derivate_Inesistente]]
- [[155_Dimostrazione_della_Gerarchia_degli_Infiniti_con_de_l_Hopital]]
- [[108_Limiti_Notevoli_di_Funzioni]]
- [[166_Approssimazioni_Polinomiali_e_Sviluppo_del_Seno]]
- [[00_MOC_Analisi_1]]

#AM1/derivate/de-l-hopital-esempi
