---
created: 2026-09-17
materia: GAL
tags:
  - materia/gal
  - tipo/nota-atomica
  - fonte/handwritten
  - lezione/2
aliases: []
---
[[00_GAL_Indice|⬅️ Torna all'Indice GAL]]

# Vettori Geometrici, Prodotto Interno ed Esterno

> Lezione 2 — 17.09.2026 (appunti OneNote «Vettori»). Si appoggia sulla [[2026-09-16-Prodotto-Cartesiano-e-Relazioni|relazione di equivalenza]] e su [[2026-09-17-Relazioni-d-Ordine-e-Funzioni|funzioni e prodotto cartesiano]]. Le stesse proprietà delle operazioni ritornano per le matrici: [[2026-09-30-Matrici-Somma-e-Prodotto-per-Scalare|somma e prodotto per scalare]].

## Segmenti orientati ed equipollenza

> **Definizione (segmento orientato).** Un **segmento orientato** (o vettore applicato) è una coppia di punti $(A,B)$ dello spazio euclideo 3-dimensionale $\mathbb{E}^3$. $A$ si chiama **punto di applicazione**.

> **Definizione (equipollenza).** Due segmenti orientati $(A,B)$ e $(C,D)$ sono **equipollenti** se i punti medi dei segmenti $AD$ e $BC$ coincidono. Si scrive $AB \triangleq CD$.

> Disegno: quadrilatero di vertici $A,B,C,D$; le diagonali $AD$ e $BC$ si incontrano nel punto medio $E$; frecce $AB$ e $CD$, lati $BD$ e $AC$ tratteggiati.

**Osservazione.** Se $A,B,C,D$ non sono collineari la condizione equivale a dire che $AB$ e $CD$ sono lati opposti di un parallelogramma $ACDB$ con lo stesso verso.

> **Proposizione.** L'equipollenza è una **relazione di equivalenza**:
> 1. $AB \triangleq AB$ (riflessiva);
> 2. $AB \triangleq CD \Rightarrow CD \triangleq AB$ (simmetrica);
> 3. $(AB \triangleq CD) \wedge (CD \triangleq EF) \Rightarrow AB \triangleq EF$ (transitiva).

La dimostrazione non è riportata negli appunti.

## Vettori come classi di equivalenza

> **Definizione (vettore).** Un **vettore** di $\mathbb{E}^3$ è una classe di equivalenza di segmenti orientati equipollenti:
> $$v = [AB] = \{\, XY \in \mathbb{E}^3 \times \mathbb{E}^3 : XY \triangleq AB \,\}$$

> Disegno: il segmento orientato $AB$ e due frecce parallele ed equipollenti in altre posizioni, a rappresentare la stessa classe.

## Operazioni tra vettori

Si fissa un'**origine** $O\in\mathbb{E}^3$ e si definiscono le operazioni sui segmenti orientati con primo estremo $O$.

1. **Zero**: il segmento orientato $OO$.
2. **Opposto**: dato $OA$ e detto $B$ il simmetrico di $A$ rispetto a $O$, l'opposto di $OA$ è $OB$.
3. **Somma**: dati $OA$ e $OB$, detto $M$ il punto medio di $AB$ e $C$ il simmetrico di $O$ rispetto a $M$, la somma è $OC$ (regola del parallelogramma).
4. **Moltiplicazione per $t\in\mathbb{R}$**: se $A=O$ allora $B=O$; se $A\neq O$ e $r$ è la retta per $O$ e $A$, $B$ è l'unico punto di $r$ di ascissa $t$ rispetto all'origine $O$ e al punto unità $A$.

> Disegni: (1) il punto $O$; (2) $OA$ e il simmetrico $OB$ da parti opposte rispetto a $O$; (3) triangolo $O,A,B$ con $M$ medio di $AB$ e $C$ simmetrico di $O$ rispetto a $M$, freccia $OC$ tratteggiata; (4) retta $r$ con $O$ in ascissa $0$, $A$ in $1$ e $B$ in $t$.

**Osservazioni.**
- La **differenza** è l'operazione derivata $OA - OB = OA + (-OB)$.
- Le operazioni tra vettori si definiscono scegliendo un'origine, operando sui rappresentanti applicati in $O$ e prendendo la classe di equipollenza del risultato: $u+v=[OA]+[OB]=[OC]$. Il risultato **non dipende dalla scelta dell'origine**.

> Disegno: parallelogramma $O,A,C,B$ con diagonale $OC$ e diagonale $AB$ tratteggiata.

### Proprietà delle operazioni

> **Proposizione.** Per ogni $u,v,w$ vettori e $s,t\in\mathbb{R}$:
> 1. $(u+v)+w=u+(v+w)$ (associativa)
> 2. $u+v=v+u$ (commutativa)
> 3. $u+0=u=0+u$
> 4. $u+(-u)=0=(-u)+u$
> 5. $1u=u$
> 6. $s(tu)=(st)u$
> 7. $t(u+v)=tu+tv$
> 8. $(s+t)u=su+tu$

Sono esattamente le proprietà che ritroveremo per le matrici.

## Sistemi di riferimento e coordinate

> **Definizione (riferimento affine).** Un **sistema di riferimento affine** in $\mathbb{E}^3$ è assegnato da 4 punti non complanari $(O,B_1,B_2,B_3)$.

Se i vettori $OB_1,OB_2,OB_3$ sono ortogonali e i segmenti $OB_1,OB_2,OB_3$ sono congruenti, il riferimento è **cartesiano**.

> Disegno: piano con origine $O$ e i punti $B_1,B_2$ nel piano, $B_3$ fuori dal piano, frecce $OB_1,OB_2,OB_3$.

**Osservazione.** Ogni riferimento affine induce una **biiezione** tra i punti di $\mathbb{E}^3$ e le terne di numeri reali, cioè gli elementi di $\mathbb{R}^3$ (vedi il [[2026-09-17-Relazioni-d-Ordine-e-Funzioni|prodotto cartesiano di più insiemi]]). Preso $X\in\mathbb{E}^3$, si considera il piano per $X$ parallelo al piano coordinato $OB_2B_3$; detto $P_1$ il punto in cui incontra l'asse $OB_1$, la lunghezza di $OP_1$ rispetto all'unità $OB_1$ è l'**ascissa** di $X$. **Ordinata** e **quota** si definiscono in modo analogo.

> Disegno: assi $OB_1,OB_2,OB_3$, piano coordinato, punto $X$ con proiezioni tratteggiate e piano parallelo a $OB_2B_3$ passante per $X$.

**Osservazione (operazioni in coordinate).** Fissato un riferimento affine, se $c(A)=(a_1,a_2,a_3)^T$ e $c(B)=(b_1,b_2,b_3)^T$ allora
$$
c(O)=\begin{pmatrix}0\\0\\0\end{pmatrix},\quad
c(-A)=\begin{pmatrix}-a_1\\-a_2\\-a_3\end{pmatrix},\quad
c(A+B)=\begin{pmatrix}a_1+b_1\\a_2+b_2\\a_3+b_3\end{pmatrix},\quad
c(tA)=\begin{pmatrix}ta_1\\ta_2\\ta_3\end{pmatrix}.
$$
(Nell'originale la seconda componente di $c(A+B)$ è $a_2+b_1$: svista evidente, corretta.)

## Prodotto interno e ortogonalità

> **Definizione (prodotto interno).** In un riferimento cartesiano, il **prodotto interno** di $u$ e $v$ è il numero reale $u\cdot v$ definito da:
> - se $u=0$ oppure $v=0$, allora $u\cdot v=0$;
> - se $u,v\neq0$, allora $u\cdot v=\|u\|\,\|v\|\cos\vartheta$,
>
> dove $\|u\|,\|v\|$ sono le lunghezze rispetto all'unità di misura e $\vartheta$ è l'angolo fra i due vettori.

> Disegno: due vettori $u$ e $v$ uscenti da $O$ con l'angolo $\vartheta$ tra essi.

> **Definizione (ortogonalità).** Due vettori $u,v$ sono **ortogonali** se l'angolo fra essi è retto; il vettore $0$ è ortogonale a tutti.

> **Proposizione.** $u\perp v \iff u\cdot v=0$.

> **Proposizione (proprietà del prodotto interno).**
> 1. $u\cdot v=v\cdot u$
> 2. $u\cdot(v_1+v_2)=u\cdot v_1+u\cdot v_2$
> 3. $(u_1+u_2)\cdot v=u_1\cdot v+u_2\cdot v$
> 4. $u\cdot u\ge0$
> 5. $u\cdot u=0\iff u=0$
> 6. $(tu)\cdot v=t(u\cdot v)=u\cdot(tv)$

### Prodotto interno in coordinate

> **Proposizione.** Fissato un riferimento cartesiano, se $u=(x_1,x_2,x_3)^T$ e $v=(y_1,y_2,y_3)^T$ allora
> $$u\cdot v=x_1y_1+x_2y_2+x_3y_3.$$

**Dimostrazione.** Si ha $u=x_1e_1+x_2e_2+x_3e_3$ e $v=y_1e_1+y_2e_2+y_3e_3$, con $e_i\cdot e_j=0$ per $i\ne j$ ed $e_i\cdot e_i=1$. Allora
$$
\begin{aligned}
u\cdot v &= \Big(\sum_{i=1}^{3}x_ie_i\Big)\cdot\Big(\sum_{j=1}^{3}y_je_j\Big)
= \sum_{i,j=1}^{3}x_iy_j\,(e_i\cdot e_j)
= \sum_{i=1}^{3}x_iy_i\,(e_i\cdot e_i)
= \sum_{i=1}^{3}x_iy_i. \qquad\blacksquare
\end{aligned}
$$
(Nell'originale $u=(x_1,x_3,x_3)^T$: svista evidente, corretta.)

> Disegno: parallelepipedo con origine $O$, versori $e_1,e_2,e_3$ e componenti $x_1,x_2,x_3$ del vettore $u$.

## Prodotto esterno e determinanti

> **Definizione (prodotto esterno).** Dati $u,v$, il **prodotto esterno** è il vettore $u\wedge v$ tale che:
> - se $u,v$ sono multipli uno dell'altro, $u\wedge v=0$;
> - se non sono collineari, $\|u\wedge v\|=\|u\|\,\|v\|\sin\vartheta$ e $u\wedge v$ giace sulla semiretta uscente da $O$ ortogonale al piano $H$ contenente $O,P,Q$ (con $u=OP$, $v=OQ$), orientata in modo che la rotazione di $u$ verso $v$ lungo $\vartheta$ risulti antioraria.

> Disegno: piano $H$ con $O,P,Q$, angolo $\vartheta$, freccia di rotazione antioraria da $u$ verso $v$ e retta ortogonale al piano con la semiretta $OS$.

Il prodotto esterno si calcola in coordinate con i **determinanti**:

$$
\begin{vmatrix}x_1&x_2\\y_1&y_2\end{vmatrix}=x_1y_2-x_2y_1,
\qquad
\begin{vmatrix}x_1&x_2&x_3\\y_1&y_2&y_3\\z_1&z_2&z_3\end{vmatrix}
= x_1\begin{vmatrix}y_2&y_3\\z_2&z_3\end{vmatrix}
- x_2\begin{vmatrix}y_1&y_3\\z_1&z_3\end{vmatrix}
+ x_3\begin{vmatrix}y_1&y_2\\z_1&z_2\end{vmatrix}.
$$

Il determinante tornerà in forma generale con lo [[2026-10-07-Inversa-Rango-Determinante-e-Eliminazione-di-Gauss|sviluppo di Laplace]].
