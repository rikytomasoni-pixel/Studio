---
tags:
  - AM1
  - successioni
  - o-piccolo
  - asintotico
  - confronti-asintotici
data: 2026-10-09
fonte: Lezione 9
stato: da_verificare
immagini_mancanti: false
---

# Proprietà degli infinitesimi equivalenti e o-piccolo

Richiamo: date $a_n, b_n$ successioni ($b_n\neq 0$ definitivamente in $n\in\mathbb{N}$):
$$\lim_{n\to\infty}\dfrac{a_n}{b_n}=0 \ \Rightarrow\ a_n=o(b_n) \ \text{ per } n\to\infty \qquad \lim_{n\to\infty}\dfrac{a_n}{b_n}=1 \ \Rightarrow\ a_n\sim b_n$$
(vedi [[41_o_piccolo_e_Asintotico]])

## Caratterizzazione dell'equivalenza asintotica

> [!abstract] Proposizione
> $$a_n\sim b_n \quad\Longleftrightarrow\quad a_n=b_n+o(b_n)$$

**dim:**
$$a_n\sim b_n \iff \lim_{n\to\infty}\dfrac{a_n}{b_n}=1 \iff \lim_{n\to\infty}\left(\dfrac{a_n}{b_n}-1\right)=0 \iff \lim_{n\to\infty}\dfrac{a_n-b_n}{b_n}=0 \iff a_n-b_n=o(b_n) \iff a_n=b_n+o(b_n)$$

**Oss:** $b_n=o(1)$ per $n\to\infty$ $\iff$ $\lim_{n\to\infty} b_n=0$ $\iff$ $b_n$ è infinitesima.

## Ulteriori proprietà di $\sim$

> [!note] Osservazione
> - $a_n\sim b_n\ \Rightarrow\ a_n, b_n$ hanno lo stesso segno definitivamente in $n\in\mathbb{N}$
> - $a_n\sim b_n$ e $b_n\to c$ $\ \Rightarrow\ a_n\to c$
> - $a_n\sim b_n \iff b_n\sim a_n$
>
> **dim (simmetria):** $\dfrac{b_n}{a_n}=\dfrac{1}{a_n/b_n}\to \dfrac{1}{1}=1$

> [!note] Osservazione
> $\sim$ è una relazione di equivalenza fra successioni (definitivamente $\neq 0$).

## Asintotici notevoli

*(fonte: foglio "Asintotici notevoli" su WeBeep)*

Per $\varepsilon_n\to 0$ ($\varepsilon_n\neq 0$ definitivamente in $n\in\mathbb{N}$), per $n\to\infty$:

$$\sin\varepsilon_n \sim \varepsilon_n, \qquad \sin\varepsilon_n = \varepsilon_n+o(\varepsilon_n)$$
$$e^{\varepsilon_n}-1 \sim \varepsilon_n, \qquad e^{\varepsilon_n}-1=\varepsilon_n+o(\varepsilon_n) \ \Rightarrow\ e^{\varepsilon_n}=1+\varepsilon_n+o(\varepsilon_n)$$
$$\log(1+\varepsilon_n)\sim\varepsilon_n, \qquad \log(1+\varepsilon_n)=\varepsilon_n+o(\varepsilon_n)$$
$$1-\cos\varepsilon_n \sim \dfrac{\varepsilon_n^2}{2}, \qquad \cos\varepsilon_n = 1-\dfrac{\varepsilon_n^2}{2}+o(\varepsilon_n^2)$$
$$(1+\varepsilon_n)^\alpha-1 \sim \alpha\,\varepsilon_n, \qquad (1+\varepsilon_n)^\alpha = 1+\alpha\,\varepsilon_n+o(\varepsilon_n)$$
$$\arctan\varepsilon_n \sim \varepsilon_n, \qquad \arctan\varepsilon_n = \varepsilon_n+o(\varepsilon_n)$$

<DUBBIO posizione="blocco ripetuto subito dopo la tabella principale, prima degli esempi finali">Il testo originale ripete una seconda volta (quasi identica) la tabella degli asintotici notevoli, introdotta da "Es: (fogli asintotici su WeBeup) Se εn→0 (εn≠0 definitivamente) allora...". Non è chiaro se si tratti di una ripetizione per promemoria durante la lezione o se contenesse una voce aggiuntiva rispetto alla prima tabella (la scansione è duplicata e di qualità peggiore).</DUBBIO>

## Proprietà di compatibilità di $\sim$ con prodotto, quoziente, potenza e limite

> [!abstract] Teorema (Proprietà)
> 1. Se $a_n\sim a_n'$ e $b_n\sim b_n'$ allora $a_n b_n \sim a_n' b_n'$
> 2. Se $a_n\sim a_n'$ e $b_n\sim b_n'$ allora $\dfrac{a_n}{b_n}\sim\dfrac{a_n'}{b_n'}$
> 3. Se $a_n\sim a_n'$, $\alpha\in\mathbb{R}$, allora $a_n^{\,\alpha}\sim (a_n')^{\,\alpha}$ (assumendo che l'operazione abbia senso)
> 4. Se $a_n\sim b_n$ allora le due successioni hanno lo stesso carattere, cioè: convergono entrambe allo stesso limite, oppure divergono entrambe a $+\infty$, oppure divergono entrambe a $-\infty$, oppure sono entrambe irregolari (non ammettono limite)

**dim:**

1. $$\dfrac{a_nb_n}{a_n'b_n'} = \dfrac{a_n}{a_n'}\cdot\dfrac{b_n}{b_n'} \to 1\cdot 1 = 1$$

2. analoga a 1) con il quoziente al posto del prodotto

3. $$\left(\dfrac{a_n}{a_n'}\right)^{\alpha} \to 1^{\alpha} = 1$$

4. Se $\exists\, \lim_{n\to\infty} a_n = l \in\overline{\mathbb{R}}$, allora $b_n = a_n\cdot\dfrac{b_n}{a_n} \to l\cdot 1 = l$, quindi $\exists\, \lim_{n\to\infty} b_n = l$.
   Se invece $\nexists\, \lim_{n\to\infty} b_n$: per assurdo supponiamo $\exists\, \lim_{n\to\infty} a_n = l$; per quanto appena dimostrato dovrebbe allora essere $\exists\, \lim_{n\to\infty} b_n = l$, assurdo. Quindi $\nexists\, \lim_{n\to\infty} a_n$. $\blacksquare$

> [!danger] Attenzione
> In generale, se $a_n\sim a_n'$ e $b_n\sim b_n'$, **non è detto** che
> $$a_n^{\,b_n} \sim (a_n')^{\,b_n'} \qquad \text{oppure} \qquad \log(a_n) \sim \log(a_n')$$

> [!danger] Attenzione
> In generale $a_n\sim b_n$ **non implica** $a_n-b_n\to 0$.

## Esempio

$$a_n = 3n^7+\log n + o(n^7) \sim 3n^7, \qquad b_n = 2n^6+o(n^6)\sim 2n^6$$
$$\Rightarrow \quad \dfrac{a_n}{b_n} \sim \dfrac{3n^7}{2n^6} = \dfrac32\, n \ \longrightarrow\ +\infty \qquad (n\to\infty)$$

## Esempio (sviluppo con radice cubica)

<DUBBIO posizione="esempio con (n^3+n^2)^(1/3) - (n^3-n)^(1/3)">Il passaggio è ricostruito a partire da appunti molto frammentati; i coefficienti numerici intermedi (in particolare l'ultimo valore del limite, trascritto in modo ambiguo tra "⅓" e "5") sono incerti.</DUBBIO>

$$a_n = \left(n^3+n^2\right)^{1/3} - \left(n^3-n\right)^{1/3}$$

Usando $a^3-b^3=(a-b)(a^2+ab+b^2)$ e gli sviluppi notevoli $(1+\varepsilon_n)^\alpha = 1+\alpha\varepsilon_n+o(\varepsilon_n)$:

$$\left(n^3+n^2\right)^{1/3} = n\left(1+\dfrac1n\right)^{1/3} = n\left(1+\dfrac{1}{3n}+o\!\left(\dfrac1n\right)\right) = n+\dfrac13+o(1)$$

$$\left(n^3-n\right)^{1/3} = n\left(1-\dfrac{1}{n^2}\right)^{1/3} = n\left(1-\dfrac{1}{3n^2}+o\!\left(\dfrac1{n^2}\right)\right) = n-\dfrac{1}{3n}+o\!\left(\dfrac1n\right)$$

$$a_n = \left(n+\dfrac13+o(1)\right) - \left(n-\dfrac{1}{3n}+o\!\left(\dfrac1n\right)\right) = \dfrac13+o(1) \ \longrightarrow\ \dfrac13 \qquad (n\to\infty)$$

## Esempio

<DUBBIO posizione="esempio con e^(1/n)-1 e arctan, poco dopo il richiamo degli asintotici notevoli">Il blocco di appunti relativo a un esempio con $a_n = e^{1/n}-1$ e uno con $\arctan$ è troppo frammentato (simboli sovrapposti, numeri di riga incerti) per essere trascritto senza rischio di errore. Andrebbe verificato sulla registrazione/slide della lezione.</DUBBIO>

## Ulteriori proprietà di o-piccolo

> [!abstract] Teorema (Proprietà)
> $$o(a_n)\cdot o(b_n) = o(a_n b_n)$$
> $$o\big(o(a_n)\big) = o(a_n)$$
> $$o\!\left(\dfrac1n\right)+o\!\left(\dfrac{1}{n^2}\right) = o\!\left(\dfrac1n\right)$$
> $$o(n)+o(n^2) = o(n^2)$$

**dim (prima proprietà):** $\dfrac{o(a_n)}{a_n}\to 0$, $\dfrac{o(b_n)}{b_n}\to 0$ per definizione, quindi $\dfrac{o(a_n)\cdot o(b_n)}{a_n\cdot b_n} = \dfrac{o(a_n)}{a_n}\cdot\dfrac{o(b_n)}{b_n}\to 0\cdot 0 = 0$.

**dim (seconda proprietà):** $o(a_n)\to 0\cdot a_n$; applicando di nuovo la definizione di $o$-piccolo a una successione che è già $o(a_n)$ si ottiene ancora $o(a_n)$.

> [!note] Osservazione
> $$a_n-b_n = o(a_n) \quad\Longleftrightarrow\quad a_n\sim b_n$$

<DUBBIO posizione="ultima pagina, dopo le proprietà di o-piccolo">La riga finale ("ad esempio o(√n)=o(n)" o simile) e l'ultimo esempio numerico della lezione, con una forma indeterminata del tipo $\left[\dfrac{0}{0}\right]$ coinvolgente $\varepsilon_n\sim 2n$ e $\sin\varepsilon_n$, sono troppo illeggibili per essere trascritti con sicurezza: mancano dati sufficienti per ricostruire la successione $a_n$ e il valore del limite richiesto ("$\lim_{n\to\infty} a_n = ?$").</DUBBIO>

### Note collegate
- [[00_MOC_Analisi_1]]
- [[41_o_piccolo_e_Asintotico]] — definizioni di o-piccolo e asintotico, gerarchia in termini di o-piccolo
- [[40_Confronti_Asintotici]] — ordine di infinito
- [[36_Gerarchia_degli_Infiniti]]
- [[37_Algebra_Limiti_Infiniti]]
- [[39_Criterio_del_Rapporto]]
- [[34_Algebra_dei_Limiti]]

#AM1/successioni-e-limiti/confronti-asintotici-proprieta-e-notevoli
