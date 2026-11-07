---
tags: [GAL, sottospazi, unione, sottospazio-somma, definizione, lezione-16]
data: 2026-11-04
lezione: 16
fonte: "GAL 2026-2027 - 20261104 - LEZIONE 16.pdf (slide 140-141)"
---

# Unione di sottospazi e sottospazio somma

## L'unione non è un sottospazio
In $\mathbb{R}^2$ siano $H=\operatorname{Span}(\underline{v})$ e $K=\operatorname{Span}(\underline{w})$ (due rette per l'origine).

> [!warning] DISEGNO NON RAPPRESENTABILE
> GAL L16 slide 140: piano cartesiano con due rette grigie per l'origine ($H$ a pendenza positiva, $K$ a pendenza negativa), un vettore rosso $\underline{v}$ su $H$, un vettore blu $\underline{w}$ su $K$ e il vettore verde $\underline{v}+\underline{w}$ (diagonale del parallelogramma) che non sta su nessuna delle due rette.

**D.** $H\cup K$ è chiuso rispetto alle operazioni? **No**: $\underline{v}+\underline{w}\notin H\cup K$.

Forse ho sbagliato a interpretare l'unione.

- **Interpretazione 1.** $H\cup K=\{\underline{v}\ |\ \underline{v}\in H\text{ oppure }\underline{v}\in K\}$
- **Interpretazione 2.** $H\cup K$ è il più piccolo insieme che contiene sia $H$ sia $K$.

Voglio, per $H,K$ sottospazi: $H\text{ "}\cup\text{" }K$ = **il più piccolo sottospazio che contiene sia $H$ sia $K$**.

## Sottospazio somma

> [!abstract] Definizione 16.2
> Sia $(V,+,\cdot)$ uno spazio vettoriale su un campo $\mathbb{K}$. Consideriamo due sottospazi vettoriali finitamente generati $H_1$ e $H_2$. Siano $\{\underline{w}_1,\dots,\underline{w}_h\}$ e $\{\underline{u}_1,\dots,\underline{u}_k\}$ due insiemi di generatori di $H_1$ e $H_2$.
>
> Definiamo **sottospazio somma** di $H_1$ e $H_2$ il sottospazio vettoriale generato dall'unione dei generatori:
> $$H_1+H_2=\operatorname{Span}\big(\underline{w}_1,\dots,\underline{w}_h,\underline{u}_1,\dots,\underline{u}_k\big)$$

> [!note] Osservazione (non presente negli appunti)
> Sulla slide le lettere degli indici dei due insiemi di generatori sono di lettura poco chiara; qui sono indicati con $h$ e $k$. Il sottospazio somma coincide con $\{\underline{a}+\underline{b}\ |\ \underline{a}\in H_1,\ \underline{b}\in H_2\}$ ed è il più piccolo sottospazio che contiene $H_1$ e $H_2$, cioè proprio il "$\cup$" cercato.

## Verso la formula di Grassmann
Possiamo sfruttare l'additività della misura: per regioni limitate del piano $A,B$
$$\mathcal{A}(A\cup B)=\mathcal{A}(A)+\mathcal{A}(B)-\mathcal{A}(A\cap B)$$
Per sottospazi vettoriali $H_1,H_2$ di $V$ vorremmo
$$\dim(H_1+H_2)=\dim(H_1)+\dim(H_2)-\dim(H_1\cap H_2)$$
→ [[135_Formula_di_Grassmann_Teorema_16_3]].

## Note collegate
- [[133_Intersezione_di_Sottospazi_Vettoriali]]
- [[96_Insieme_di_Generatori]]
- [[95_Combinazioni_Lineari_e_Span]]
- [[94_Sottospazi_Vettoriali]]
- [[135_Formula_di_Grassmann_Teorema_16_3]]
- Indice: [[17_Indice_Lezione_16]] · [[00_MOC_GAL]]

#GAL/sottospazi/somma
