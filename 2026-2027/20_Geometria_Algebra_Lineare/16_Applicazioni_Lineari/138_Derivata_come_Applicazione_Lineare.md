---
tags: [GAL, applicazioni-lineari, esempi, derivata, spazi-di-funzioni, lezione-17]
data: 2026-11-05
lezione: 17
fonte: "GAL 2026-2027 - 20261105 - LEZIONE 17.pdf (slide 150)"
---

# Esempio (IV): la derivata come applicazione lineare tra spazi di funzioni

$$V=\mathcal{C}^1(I)=\{f:I\to\mathbb{R}\ |\ f\text{ derivabile in ogni punto di }I\}$$
$$W=\mathcal{C}^0(I)=\{f:I\to\mathbb{R}\ |\ f\text{ continua in ogni punto di }I\}$$
($\mathcal{C}$ maiuscola corsiva: iniziale di *Continuo*.)

$$D:\mathcal{C}^1(I)\to\mathcal{C}^0(I),\qquad f\mapsto f'=\text{la derivata di }f$$

$D$ è un'applicazione lineare tra spazi di funzioni:
$$(f+g)'=f'+g'\qquad(\lambda f)'=\lambda f'$$

> [!note] Osservazione (non presente negli appunti)
> Perché $D$ abbia davvero valori in $\mathcal{C}^0(I)$ serve che $f'$ sia continua, cioè $\mathcal{C}^1(I)$ nel senso usuale (derivata continua). Nell'enunciato della slide $\mathcal{C}^1(I)$ è descritto come "derivabile in ogni punto di $I$".

## Esempio
$$\mathcal{C}^0(\mathbb{R})=\{x^2+x-1,\ \cos(x),\ \sin(x),\ e^x,\ |x|,\dots\}$$
$$\mathcal{C}^1(\mathbb{R})=\{x^2+x-1,\ \cos(x),\ \sin(x),\ e^x,\ \cancel{|x|},\dots\}$$
($|x|$ è continua ma non derivabile in $0$, quindi è barrata in $\mathcal{C}^1(\mathbb{R})$.)

> [!warning] DISEGNO NON RAPPRESENTABILE
> GAL L17 slide 150: sotto $\mathcal{C}^0(\mathbb{R})$ quattro piccoli grafici associati alle funzioni: parabola (U), onda sinusoidale, curva crescente (esponenziale) e "V" (valore assoluto).

$$\mathcal{C}^\infty(\mathbb{R})\subseteq\dots\subseteq\mathcal{C}^2(\mathbb{R})\subseteq\mathcal{C}^1(\mathbb{R})\subseteq\mathcal{C}^0(\mathbb{R})$$

$D:\mathcal{C}^1(\mathbb{R})\to\mathcal{C}^0(\mathbb{R})$:
$$D(x^2+x-1)=2x+1\qquad D(\sin(x))=\cos(x)\qquad D(e^x)=e^x$$

## Note collegate
- [[136_Applicazioni_Lineari_Definizione_17_1]]
- [[92_Esempi_di_Spazi_Vettoriali]]
- [[120_Spazi_Vettoriali_Finitamente_Generati_e_Non]]
- Indice: [[18_Indice_Lezione_17]] · [[00_MOC_GAL]]

#GAL/applicazioni-lineari/derivata
