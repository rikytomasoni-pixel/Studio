---
tags:
  - AM1
  - taylor
  - maclaurin
  - sviluppi-notevoli
data: 2026-11-25
lezione: 21
fonte: "AM1 L21 26-27.pdf (pag. 7-8)"
---

# Sviluppi di Maclaurin di $e^x$, $\sin x$, $\cos x$

Per $x\to0$ (formula di Maclaurin, [[168_Teorema_di_Taylor_con_Resto_di_Peano]]):

> [!abstract] Esponenziale
> $f(x)=e^x$ ha $f^{(n)}(x)=e^x$ per ogni $n\in\mathbb{N}$, quindi $f^{(n)}(0)=1$ e
> $$e^x=\sum_{k=0}^n\frac{x^k}{k!}+o(x^n)\qquad x\to0$$

> [!abstract] Seno e coseno
> $$\sin x=x-\frac{x^3}{3!}+\frac{x^5}{5!}-\frac{x^7}{7!}+\dots+(-1)^n\frac{x^{2n+1}}{(2n+1)!}+o\big(x^{2n+2}\big)$$
> $$\cos x=1-\frac{x^2}{2!}+\frac{x^4}{4!}-\frac{x^6}{6!}+\frac{x^8}{8!}+\dots+(-1)^n\frac{x^{2n}}{(2n)!}+o\big(x^{2n+1}\big)$$

> [!info] Indicazione del docente
> Gli sviluppi notevoli delle funzioni elementari sono sul **libro di testo** e nel **file caricato sulla pagina WeBeep del corso**: da consultare lì.

> [!note] Osservazione (non presente negli appunti)
> Per $\sin x$ l'ultimo termine scritto ha grado $2n+1$ e il resto è $o(x^{2n+2})$ (e non solo $o(x^{2n+1})$) perché il termine di grado $2n+2$ è nullo; analogamente per $\cos x$ con $o(x^{2n+1})$. Per $n=1$ il seno ridà $x-\frac{x^3}{6}$ con resto $o(x^4)$, più preciso di quanto visto in [[166_Approssimazioni_Polinomiali_e_Sviluppo_del_Seno]].

Usi: [[176_Esempio_Limite_con_Sviluppi_di_Taylor]], [[177_Esempio_Sviluppo_di_e_alla_x_quadro]].

## Note collegate
- [[167_Polinomio_di_Taylor]]
- [[166_Approssimazioni_Polinomiali_e_Sviluppo_del_Seno]]
- [[179_Serie_di_Taylor]]
- [[108_Limiti_Notevoli_di_Funzioni]]
- [[00_MOC_Analisi_1]]

#AM1/taylor/maclaurin
