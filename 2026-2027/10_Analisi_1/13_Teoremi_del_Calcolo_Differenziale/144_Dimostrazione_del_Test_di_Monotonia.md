---
tags:
  - AM1
  - derivate
  - monotonia
  - teorema
  - dimostrazione
data: 2026-11-18
lezione: 19
fonte: "AM1 L19 26-27.pdf (pag. 5-8)"
---

# Dimostrazione del test di monotonia

Dimostrazione del [[140_Test_di_Monotonia|teorema (test di monotonia)]] (**D23**, insieme alla [[143_Caratterizzazione_delle_Funzioni_Costanti_su_un_Intervallo|caratterizzazione delle funzioni costanti]]).

> [!info] Solo il caso crescente
> Per semplicità si considerano solo i casi in cui $f$ è crescente (se $f$ è decrescente la dimostrazione è analoga).

## Passo 1: $f$ crescente e derivabile $\Rightarrow f'(x)\ge0$

Sia $f:(a,b)\to\mathbb{R}$ derivabile e crescente in $(a,b)$. Vogliamo mostrare che $f'(x)\ge0$ per ogni $x\in(a,b)$ (sarà conseguenza del [[101_Teorema_di_Permanenza_del_Segno_per_Funzioni|teorema di permanenza del segno]]).

Sia $x\in(a,b)$ e sia $h\in\mathbb{R}$ con $|h|\ne0$ abbastanza piccolo in modo che $x+h\in(a,b)$.
- $h>0\ \Rightarrow\ x+h>x\ \Rightarrow\ f(x+h)\ge f(x)$
- $h<0\ \Rightarrow\ x+h<x\ \Rightarrow\ f(x+h)\le f(x)$

Allora, per ogni $h\ne0$,
$$\frac{f(x+h)-f(x)}{h}\ge0\tag{$*$}$$
Poiché $f$ è derivabile esiste finito
$$f'(x)=\lim_{h\to0}\frac{f(x+h)-f(x)}{h}$$
e per permanenza del segno da $(*)$ segue che $f'(x)\ge0$ per ogni $x\in(a,b)$.

## Passo 2: $f'(x)\ge0$ in $(a,b)\Rightarrow f$ crescente

Se $f:(a,b)\to\mathbb{R}$ è derivabile in $(a,b)$ con $f'(x)\ge0$ per ogni $x\in(a,b)$, allora $f$ è crescente in $(a,b)$ (segue dal [[142_Teorema_di_Lagrange|teorema di Lagrange]]).

Siano $x_1,x_2\in(a,b)$ con $x_1<x_2$. Vogliamo mostrare che $f(x_1)\le f(x_2)$. Poiché $[x_1,x_2]\subset(a,b)$ ed essendo $f$ derivabile (e quindi continua, [[129_Derivabilita_e_Continuita]]) in $(a,b)$, avremo che $f$ è continua e derivabile in $[x_1,x_2]$.

Per il teorema del valor medio di Lagrange applicato a $f:[x_1,x_2]\to\mathbb{R}$ esiste $c\in(x_1,x_2)$ tale che
$$\frac{f(x_2)-f(x_1)}{x_2-x_1}=f'(c)\ge0$$
perché $f'(x)\ge0$ per ogni $x\in(a,b)$ per ipotesi. Quindi, poiché $x_2>x_1$,
$$f(x_2)-f(x_1)=\underbrace{f'(c)}_{\ge0}\underbrace{(x_2-x_1)}_{\ge0}\ge0\ \Rightarrow\ f(x_2)\ge f(x_1)$$
Poiché ciò è vero per ogni $x_1,x_2\in(a,b)$ con $x_1<x_2$, per definizione $f$ è crescente in $(a,b)$.

## Passo 3: $f'(x)>0$ in $(a,b)\Rightarrow f$ strettamente crescente

Se $f:(a,b)\to\mathbb{R}$ è derivabile e $f'(x)>0$ per ogni $x\in(a,b)$, vogliamo mostrare che $f$ è strettamente crescente in $(a,b)$.

Come prima, se $x_1,x_2\in(a,b)$ con $x_1<x_2$, per il teorema del valor medio di Lagrange esiste $c\in(x_1,x_2)\subset(a,b)$ tale che
$$\frac{f(x_2)-f(x_1)}{x_2-x_1}=f'(c)>0\ \Rightarrow\ f(x_2)-f(x_1)=\underbrace{f'(c)}_{>0}\underbrace{(x_2-x_1)}_{>0}>0\ \Rightarrow\ f(x_2)>f(x_1)$$
Poiché ciò è vero per ogni $x_1,x_2\in(a,b)$ con $x_1<x_2$, per definizione $f$ è strettamente crescente in $(a,b)$. $\square$

## Conseguenza: invertibilità

> [!note] Osservazione
> Se $f:(a,b)\to\mathbb{R}$ è derivabile in $(a,b)$ allora
> $$f'(x)>0\ \text{in }(a,b)\ \ \big(f'(x)<0\ \text{in }(a,b)\big)\ \Rightarrow\ f\text{ è strettamente crescente (decrescente) in }(a,b)\ \Rightarrow\ f\text{ è invertibile in }(a,b)$$
> L'ultima implicazione è il teorema sulle [[27_Teorema_Monotone_Invertibili|funzioni strettamente monotone]].

## Note collegate
- [[140_Test_di_Monotonia]]
- [[145_Test_di_Monotonia_Controesempi_e_Osservazioni]]
- [[142_Teorema_di_Lagrange]]
- [[143_Caratterizzazione_delle_Funzioni_Costanti_su_un_Intervallo]]
- [[101_Teorema_di_Permanenza_del_Segno_per_Funzioni]]
- [[129_Derivabilita_e_Continuita]]
- [[27_Teorema_Monotone_Invertibili]]
- [[00_MOC_Analisi_1]]

#AM1/derivate/test-monotonia-dimostrazione
