---
tags:
  - AM1
  - taylor
  - esempio
  - sviluppi-composti
data: 2026-11-25
lezione: 21
fonte: "AM1 L21 26-27.pdf (pag. 15)"
---

# Esempio: sviluppo di $e^{x^2}$ al quarto ordine in $0$

Si parte da $e^t=1+t+\dfrac{t^2}{2}+\dfrac{t^3}{6}+\dfrac{t^4}{24}+o(t^4)$ per $t\to0$ e si pone $t=x^2$:
$$f(x)=e^{x^2}=1+x^2+\frac{x^4}{2}+\frac{x^6}{6}+\frac{x^8}{24}+o(x^8)=1+x^2+\frac{x^4}{2}+o(x^4)$$

I termini di grado $>4$ vengono assorbiti nel resto $o(x^4)$ ([[178_Algebra_degli_o_piccoli]]).

> [!note] Osservazione (non presente negli appunti)
> Per l'[[173_Taylor_Peano_Unicita_e_Controesempio_senza_Derivate_Successive|unicità]] dello sviluppo, questo coincide con il polinomio di Taylor $P_4$ di $e^{x^2}$ in $0$ (senza calcolare le derivate quarte).

## Note collegate
- [[172_Sviluppi_di_Maclaurin_di_e_alla_x_sin_cos]]
- [[176_Esempio_Limite_con_Sviluppi_di_Taylor]]
- [[00_MOC_Analisi_1]]

#AM1/taylor/sviluppi-composti
