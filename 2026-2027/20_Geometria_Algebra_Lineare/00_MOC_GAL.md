---
tags: [GAL, MOC, indice-generale]
data: 2026-11-12
lezione: 0-20
fonte: "Tutti i PDF GAL 2026-2027 (Lezioni 0-4, 6-7, 9-11, 13, 15-17 e 19-20)"
---

# MOC — Geometria e Algebra Lineare A.A. 2026-2027

Mappa dei contenuti (Zettelkasten). Ordine cronologico delle lezioni, poi mappa tematica.

```mermaid
flowchart LR
    A[Fondamenti teorici] --> B[Vettori geometrici]
    A --> C[Matrici]
    C --> D[Matrice inversa]
    C --> E[Metodo di eliminazione di Gauss]
    E --> F[Rango]
    E --> G[Determinante]
    D --> G
    E --> H[Sistemi lineari]
    H --> I[Spazi affini]
    I --> J[Spazi vettoriali]
    J --> K[Indipendenza lineare, basi e dimensione]
    K --> L[Somma, intersezione e Grassmann]
    K --> M[Applicazioni lineari]
```

Struttura cartelle: `01_Fondamenti_Teorici` · `02_Vettori_Geometrici` · `03_Matrici` · `04_Matrice_Inversa` · `05_Metodo_di_Eliminazione_di_Gauss` · `06_Rango` · `07_Determinante` · `08_Applicazioni` · `09_Organizzazione` · `10_Indici_Lezioni` · `11_Sistemi_Lineari` · `12_Spazi_Affini` · `13_Spazi_Vettoriali` · `14_Indipendenza_Lineare_Basi_Dimensione` · `15_Somma_Intersezione_e_Grassmann` · `16_Applicazioni_Lineari`

## Linea cronologica

| Lezione | Data | Argomenti principali | Link |
|---|---|---|---|
| 0 | 2026-09-16 | Introduzione al corso; prodotto cartesiano; relazione binaria; relazione di equivalenza | [[01_Indice_Lezione_0]] |
| 1 | 2026-09-17 | Relazioni d'ordine; funzioni; iniettività e suriettività; prodotto cartesiano di più insiemi | [[02_Indice_Lezione_1]] |
| 2 | 2026-09-17 | Vettori geometrici (appunti OneNote «Vettori»): equipollenza, operazioni, coordinate, prodotto interno ed esterno, determinanti | [[03_Indice_Lezione_2]] |
| 3 | 2026-09-30 | Matrici: definizione ed esempi; campo F2; somma tra matrici; prodotto tra uno scalare e una matrice | [[04_Indice_Lezione_3]] |
| 4 | 2026-10-01 | Prodotto matriciale righe per colonne; il prodotto codifica la composizione di funzioni; PageRank (parte 1); identità e diagonali | [[05_Indice_Lezione_4]] |
| 5 | — | (nessun PDF fornito: la numerazione delle slide prosegue senza interruzione, L4 termina a 44 e L6 inizia a 45) | — |
| 6 | 2026-10-07 | Matrice invertibile; rango; determinante (sviluppo di Laplace); matrici triangolari; metodo di eliminazione di Gauss; pivot e matrice a scala | [[07_Indice_Lezione_6]] |
| 7 | 2026-10-08 | Reversibilità del MEG; codifica del MEG con il prodotto matriciale; rango con il MEG; teorema di Binet; determinante con il MEG; proprietà del determinante | [[08_Indice_Lezione_7]] |
| Es. 5.1 | 2026-10-09 | Esercizi: calcolo del determinante con MEG, Laplace e metodo misto (solo matrice A svolta) | [[103_Esercizio_5_1_Calcolo_del_Determinante]] |
| Es. EE1 | 2026-10-09 | Esercizio: matrice come somma di $r$ matrici di rango 1 (MEG, matrici elementari, $A=PLU$) | [[108_Esercizio_EE1_Somma_di_Matrici_di_Rango_1]] |
| 8 | — | (nessun PDF fornito: la numerazione delle slide prosegue senza interruzione, L7 termina a 72 e L9 inizia a 73) | — |
| 9 | 2026-10-12 | Rappresentazioni matriciali di un sistema lineare; risoluzione via MEG; teorema di Rouché-Capelli | [[10_Indice_Lezione_9]] |
| 10 | 2026-10-14 | Commenti a Rouché-Capelli; nucleo; teorema di struttura; teorema di Cramer; ricerca della matrice inversa; teorema sull'invertibilità | [[11_Indice_Lezione_10]] |
| 11 | 2026-10-15 | Spazi affini (cartesiane e parametriche); spazio vettoriale: definizione ed esempi; sottospazi vettoriali | [[12_Indice_Lezione_11]] |
| 12 | — | (nessun PDF fornito: la numerazione delle slide prosegue senza interruzione, L11 termina a 107 e L13 inizia a 108) | — |
| 13 | 2026-10-19 | Combinazioni lineari e span; generatori; vettori linearmente indipendenti; base; teorema di unicità della rappresentazione; dimensione | [[14_Indice_Lezione_13]] |
| 14 | — | (nessun PDF fornito: la numerazione delle slide prosegue senza interruzione, L13 termina a 118 e L15 inizia a 119) | — |
| 15 | 2026-10-28 | Lemma fondamentale; teorema della dimensione; significato della dimensione; spazi finitamente generati; basi canoniche; estrazione e completamento di una base; fac-simile d'esame | [[16_Indice_Lezione_15]] |
| 16 | 2026-11-04 | Riepilogo sul rango; spazio delle righe e delle colonne; la dimensione come misura; intersezione e somma di sottospazi; formula di Grassmann | [[17_Indice_Lezione_16]] |
| 17 | 2026-11-05 | Applicazioni lineari (definizione, esempi, proprietà); composizione e inversione; come definire un'applicazione lineare su una base | [[18_Indice_Lezione_17]] |
| 18 | — | (nessun PDF fornito: la numerazione delle slide prosegue senza interruzione, L17 termina a 155 e L19 inizia a 156) | — |
| 19 | 2026-11-11 | Analisi esiti prova in itinere; immagine e controimmagine di sottospazi; immagine di un'applicazione lineare; suriettività | [[20_Indice_Lezione_19]] |
| 20 | 2026-11-12 | Nucleo e criterio di iniettività; teorema della fibra; isomorfismi; teorema di isomorfismo; mappa delle coordinate e di parametrizzazione | [[21_Indice_Lezione_20]] |

## Fondamenti teorici — insiemi, relazioni, funzioni
- [[11_Prodotto_Cartesiano]] — Prodotto cartesiano *(L0)*
- [[12_Relazione_Binaria]] — Relazione binaria *(L0)*
- [[13_Proprieta_Riflessiva_Simmetrica_Transitiva]] — Proprietà riflessiva, simmetrica e transitiva *(L0)*
- [[14_Relazione_di_Equivalenza]] — Relazione di equivalenza *(L0)*
- [[15_Relazione_di_Ordine]] — Relazione d'ordine *(L1)*
- [[16_Funzioni]] — Funzioni *(L1)*
- [[17_Excursus_Logico_Negazione_Implicazione]] — Excursus logico: negazione di un'implicazione *(L1)*
- [[18_Iniettivita_Suriettivita_Biettivita]] — Iniettività, suriettività e biettività *(L1)*
- [[19_Prodotto_Cartesiano_di_Piu_Insiemi]] — Prodotto cartesiano di più insiemi *(L1)*
- [[31_Il_Campo_F2]] — Il campo $\mathbb{F}_2$ *(L3)*

## Vettori geometrici (precursori di spazi vettoriali e prodotto scalare)
- [[20_Segmenti_Orientati_ed_Equipollenza]] — Segmenti orientati ed equipollenza *(L2)*
- [[21_Vettori_come_Classi_di_Equivalenza]] — Vettori come classi di equivalenza *(L2)*
- [[22_Operazioni_tra_Vettori]] — Operazioni tra vettori *(L2)*
- [[23_Sistemi_di_Riferimento_e_Coordinate]] — Sistemi di riferimento e coordinate *(L2)*
- [[24_Proprieta_delle_Operazioni_tra_Vettori]] — Proprietà delle operazioni tra vettori *(L2)*
- [[25_Prodotto_Interno_e_Ortogonalita]] — Prodotto interno e ortogonalità *(L2)*
- [[26_Prodotto_Interno_in_Coordinate]] — Prodotto interno in coordinate *(L2)*
- [[27_Prodotto_Esterno]] — Prodotto esterno *(L2)*
- [[28_Determinanti_2x2_e_3x3]] — Determinanti 2×2 e 3×3 *(L2)*

## Matrici e algebra delle matrici
- [[30_Matrici_come_Rappresentazione_di_Funzioni]] — Matrici come rappresentazione di funzioni *(L3)*
- [[32_Definizione_di_Matrice]] — Definizione di matrice *(L3)*
- [[33_Matrici_Casi_Speciali]] — Notazione e casi speciali di matrici *(L3)*
- [[34_Confronto_e_Uguaglianza_tra_Matrici]] — Confronto e uguaglianza tra matrici *(L3)*
- [[35_Somma_tra_Matrici]] — Somma tra matrici *(L3)*
- [[40_Opposto_di_una_Matrice]] — Opposto di una matrice *(L4)*
- [[36_Prodotto_di_una_Matrice_per_uno_Scalare]] — Prodotto di una matrice per uno scalare *(L3)*
- [[37_Efficienza_Computazionale]] — Efficienza computazionale e proprietà delle operazioni *(L3)*
- [[41_Prodotto_Matriciale_Righe_per_Colonne]] — Prodotto matriciale righe per colonne *(L4)*
- [[42_Prodotto_e_Composizione_di_Funzioni]] — Il prodotto codifica la composizione di funzioni *(L4)*
- [[44_Proprieta_del_Prodotto_Matriciale]] — Proprietà del prodotto matriciale *(L4)*
- [[45_Matrice_Identita_e_Matrici_Diagonali]] — Matrice identità e matrici diagonali *(L4)*

## Applicazioni
- [[43_PageRank_e_Matrice_di_Google]] — PageRank e matrice di Google (parte 1) *(L4)*

## Organizzazione
- [[10_Organizzazione_del_Corso]] — Organizzazione del corso *(L0)*
- [[145_Analisi_degli_Esiti_della_Prova_in_Itinere]] — Analisi degli esiti della prova in itinere *(L19)*

## Matrice inversa e prodotto matriciale (Lezioni 6-7)
- [[60_Matrice_Invertibile]] — Matrice invertibile *(L6)*
- [[61_Unicita_e_Bilateralita_dell_Inversa]] — Unicità e bilateralità dell'inversa *(L6)*
- [[62_Non_Commutativita_del_Prodotto_Matriciale]] — Non commutatività del prodotto matriciale *(L6)*
- [[72_Esistenza_della_Matrice_Inversa]] — Esistenza della matrice inversa *(L7)*
- [[87_Ricerca_della_Matrice_Inversa]] — Ricerca della matrice inversa *(L10)*
- [[88_Teorema_sull_Invertibilita_della_Matrice]] — Teorema sull'invertibilità della matrice *(L10)*

## Rango
- [[63_Rango_di_una_Matrice]] — Rango di una matrice *(L6)*
- [[64_Rango_e_Matrice_di_Probabilita_Congiunta]] — Rango e matrice di probabilità congiunta *(L6)*
- [[73_MEG_e_Rango]] — MEG e rango *(L7)*
- [[108_Esercizio_EE1_Somma_di_Matrici_di_Rango_1]] — Esercizio EE1: somma di matrici di rango 1 *(esercizi 09-10)*
- [[109_EE1_Riduzione_a_Scala_di_A]] — EE1: riduzione a scala *(esercizi 09-10)*
- [[110_EE1_Fattorizzazione_con_Matrici_Elementari]] — EE1: matrici elementari e $A=PLU$ *(esercizi 09-10)*
- [[111_EE1_Somma_di_Tre_Matrici_di_Rango_1]] — EE1: somma di tre matrici di rango 1 *(esercizi 09-10)*
- [[130_Riepilogo_sulle_Definizioni_di_Rango]] — Riepilogo sulle definizioni di rango *(L16)*
- [[131_Spazio_delle_Righe_e_delle_Colonne]] — Spazio delle righe e delle colonne, $r(A)=\dim\operatorname{col}(A)$ *(L16)*

## Determinante
- [[65_Determinante_Sviluppo_di_Laplace]] — Determinante: sviluppo di Laplace *(L6)*
- [[66_Matrici_Triangolari]] — Matrici triangolari e loro determinante *(L6)*
- [[74_Teorema_di_Binet]] — Teorema di Binet *(L7)*
- [[75_Calcolo_del_Determinante_con_il_MEG]] — Calcolo del determinante con il MEG *(L7)*
- [[76_Determinante_Normalizzato_e_Alternante]] — Determinante normalizzato e alternante *(L7)*
- [[77_Determinante_Multilineare]] — Determinante multilineare *(L7)*
- [[78_Determinante_e_Sostituzione]] — Determinante e operazione di sostituzione *(L7)*
- [[79_Determinante_con_Righe_Uguali]] — Determinante con righe uguali *(L7)*
- [[103_Esercizio_5_1_Calcolo_del_Determinante]] — Esercizio 5.1: calcolo del determinante *(esercizi 09-10)*
- [[104_Determinante_con_il_MEG_Esempio_con_Scambio_di_Righe]] — Esempio con il MEG e scambio di righe *(esercizi 09-10)*
- [[105_Determinante_Laplace_Esempio_3x3_Riga_3]] — Esempio con Laplace sulla riga 3 *(esercizi 09-10)*
- [[106_Determinante_Metodo_Misto_MEG_e_Laplace]] — Metodo misto MEG + Laplace *(esercizi 09-10)*
- [[107_Confronto_Metodi_Calcolo_Determinante]] — Confronto tra i metodi *(esercizi 09-10)*

## Metodo di eliminazione di Gauss (MEG)
- [[67_Operazioni_Elementari_sulle_Righe]] — Operazioni elementari sulle righe *(L6)*
- [[68_Metodo_di_Eliminazione_di_Gauss]] — Metodo di eliminazione di Gauss (MEG) *(L6)*
- [[69_Pivot_e_Matrice_a_Scala]] — Pivot e matrice a scala *(L6)*
- [[70_Reversibilita_del_MEG]] — Reversibilità del MEG *(L7)*
- [[71_Codifica_del_MEG_con_il_Prodotto_Matriciale]] — Codifica del MEG con il prodotto matriciale *(L7)*

## Sistemi lineari
- [[80_Rappresentazioni_Matriciali_di_un_Sistema_Lineare]] — Rappresentazioni matriciali di un sistema lineare *(L9)*
- [[81_Risoluzione_di_un_Sistema_con_MEG_Esempio_Parametrico]] — Risoluzione con il MEG: esempio con parametri *(L9)*
- [[82_Teorema_di_Rouche_Capelli]] — Teorema di Rouché-Capelli *(L9)*
- [[83_Esempio_Sistema_con_Parametro_k_e_Rouche_Capelli]] — Esempio con parametro k *(L10)*
- [[84_Nucleo_e_Sistema_Omogeneo_Associato]] — Nucleo e sistema omogeneo associato *(L10)*
- [[85_Teorema_di_Struttura_delle_Soluzioni]] — Teorema di struttura delle soluzioni *(L10)*
- [[86_Teorema_di_Cramer]] — Teorema di Cramer *(L10)*
- [[112_Esercizio_5_4_Sistemi_con_Parametro]] — Esercizio 5.4: sistemi con parametro *(esercizi)*
- [[113_Esercizio_5_4_i_Determinante_Sempre_Nullo]] — 5.4 (i): determinante sempre nullo *(esercizi)*
- [[114_Esercizio_5_4_ii_Cramer_e_Caso_Singolare]] — 5.4 (ii): Cramer e caso singolare *(esercizi)*
- [[115_Esercizio_5_4_iii_Quattro_Equazioni_Tre_Incognite]] — 5.4 (iii): 4 equazioni, 3 incognite *(esercizi)*
- [[116_Strategia_Determinante_per_Sistemi_con_Parametro]] — Strategia: determinante e parametri *(osservazione)*

## Spazi affini
- [[89_Interpretazione_Geometrica_dei_Sistemi_Lineari_Spazi_Affini]] — Interpretazione geometrica dei sistemi lineari *(L11)*
- [[90_Sistemi_Omogenei_e_Chiusura_della_Somma]] — Sistemi omogenei e chiusura della somma *(L11)*

## Spazi vettoriali
- [[91_Spazio_Vettoriale_Definizione]] — Spazio vettoriale: definizione *(L11)*
- [[92_Esempi_di_Spazi_Vettoriali]] — Esempi di spazi vettoriali *(L11)*
- [[93_Proprieta_Fondamentali_degli_Spazi_Vettoriali]] — Proprietà fondamentali degli spazi vettoriali *(L11)*
- [[94_Sottospazi_Vettoriali]] — Sottospazi vettoriali *(L11)*
- [[95_Combinazioni_Lineari_e_Span]] — Combinazioni lineari e span *(L13)*
- [[96_Insieme_di_Generatori]] — Insieme di generatori *(L13)*
- [[97_Esempio_Generatori_di_R3_e_Rappresentazioni_Multiple]] — Esempio: generatori di R3 e rappresentazioni multiple *(L13)*

## Indipendenza lineare, basi e dimensione
- [[98_Vettori_Linearmente_Indipendenti]] — Vettori linearmente indipendenti *(L13)*
- [[99_Dipendenza_Lineare_e_Vettori_Ridondanti]] — Dipendenza lineare e vettori ridondanti *(L13)*
- [[100_Base_di_uno_Spazio_Vettoriale]] — Base di uno spazio vettoriale *(L13)*
- [[101_Teorema_di_Unicita_della_Rappresentazione_rispetto_a_una_Base]] — Teorema di unicità della rappresentazione *(L13)*
- [[102_Dimensione_di_uno_Spazio_Vettoriale]] — Dimensione di uno spazio vettoriale *(L13)*
- [[117_Lemma_Fondamentale_Teorema_15_1]] — Lemma fondamentale (Teorema 15.1) *(L15)*
- [[118_Teorema_della_Dimensione_Teorema_15_2]] — Teorema della dimensione (Teorema 15.2) *(L15)*
- [[119_Significato_della_Dimensione_Massimo_Indipendenti_e_Minimo_Generatori]] — Significato della dimensione *(L15)*
- [[120_Spazi_Vettoriali_Finitamente_Generati_e_Non]] — Spazi vettoriali finitamente generati e non *(L15)*
- [[121_Basi_Canoniche]] — Basi canoniche *(L15)*
- [[122_Estrazione_e_Completamento_Due_Problemi_Classici]] — Estrazione e completamento: due problemi classici *(L15)*
- [[123_Base_per_Costruzione_Libera_con_il_MEG_sulle_Righe]] — Base per costruzione libera: MEG sulle righe *(L15)*
- [[124_Estrazione_di_una_Base_con_i_Pivot_delle_Colonne]] — Estrazione di una base: pivot delle colonne *(L15)*
- [[125_Completamento_ad_una_Base]] — Completamento ad una base *(L15)*
- [[126_Fac_simile_28_10_Esercizio_su_Sottospazi_Dimensione_e_Basi]] — Fac-simile 28-10: sottospazi, dimensione e basi *(esercizi)*
- [[127_Fac_simile_i_V_e_un_Sottospazio_Due_Strategie]] — Fac-simile (i): $V$ è un sottospazio *(esercizi)*
- [[128_Fac_simile_ii_Dimensione_e_Basi_di_V_e_W]] — Fac-simile (ii): dimensione e basi di $V$ e $W$ *(esercizi)*
- [[129_Fac_simile_iii_Identita_come_Somma_di_un_Elemento_di_V_e_di_W]] — Fac-simile (iii): $\mathrm{Id}_2=A_1+A_2$ *(esercizi)*
- [[132_Significato_della_Dimensione_Seconda_Parte]] — Significato della dimensione (II): la dimensione è una misura *(L16)*

## Somma, intersezione e formula di Grassmann
- [[133_Intersezione_di_Sottospazi_Vettoriali]] — Intersezione di sottospazi *(L16)*
- [[134_Unione_di_Sottospazi_e_Sottospazio_Somma]] — Unione di sottospazi e sottospazio somma *(L16)*
- [[135_Formula_di_Grassmann_Teorema_16_3]] — Formula di Grassmann (Teorema 16.3) *(L16)*

## Applicazioni lineari
- [[136_Applicazioni_Lineari_Definizione_17_1]] — Applicazioni lineari (Definizione 17.1) *(L17)*
- [[137_Esempi_di_Applicazioni_Lineari_Matrici_Trasposizione_Traccia]] — Esempi: $L_A$, trasposizione, traccia *(L17)*
- [[138_Derivata_come_Applicazione_Lineare]] — La derivata come applicazione lineare *(L17)*
- [[139_Proprieta_delle_Applicazioni_Lineari]] — Proprietà: $L(\underline{0})=\underline{0}$, combinazioni lineari *(L17)*
- [[140_Esempi_e_Controesempi_di_Applicazioni_Lineari]] — Esempi e controesempi *(L17)*
- [[141_Composizione_e_Inversione_di_Applicazioni_Lineari]] — Composizione e inversione: $L_B\circ L_A=L_{BA}$ *(L17)*
- [[142_Come_Definire_una_Applicazione_Lineare_Proposizione_17_2]] — Come definire un'applicazione lineare (Prop. 17.2) *(L17)*
- [[143_Esempio_Applicazione_Lineare_da_Polinomi_a_Matrici]] — Esempio: $\mathbb{R}[t]_{\le2}\to M(2,2)$ *(L17)*
- [[144_Applicazioni_Lineari_da_Kn_a_Km_e_Matrice_Associata]] — Applicazioni $\mathbb{K}^n\to\mathbb{K}^m$ e matrice associata *(L17)*
- [[146_Immagine_e_Controimmagine_di_Sottospazi_Vettoriali]] — Immagine e controimmagine di sottospazi *(L19)*
- [[147_Immagine_di_una_Applicazione_Lineare_e_Suriettivita]] — Immagine di un'applicazione lineare e suriettività *(L19)*
- [[148_Proposizione_19_1_Immagine_dei_Generatori]] — Proposizione 19.1: immagine dei generatori *(L19)*
- [[149_Conseguenze_della_Suriettivita_Generatori_e_Dimensione]] — Conseguenze della suriettività: generatori e dimensione *(L19)*
- [[150_Suriettivita_di_L_A_e_Spazio_delle_Colonne]] — Suriettività di $L_A$ e spazio delle colonne *(L19)*
- [[151_Nucleo_di_una_Applicazione_Lineare]] — Nucleo di un'applicazione lineare *(L20)*
- [[152_Teorema_20_1_Criterio_di_Iniettivita]] — Teorema 20.1 (criterio di iniettività) *(L20)*
- [[153_Conseguenze_del_Criterio_di_Iniettivita_L_A_e_Rango]] — Conseguenze del criterio: $L_A$ e rango *(L20)*
- [[154_Corollario_20_2_Iniettivita_e_Indipendenza_Lineare]] — Corollario 20.2: iniettività e indipendenza lineare *(L20)*
- [[155_Teorema_20_3_Teorema_della_Fibra]] — Teorema 20.3 (teorema della fibra) *(L20)*
- [[156_Isomorfismi_Definizione_20_4_e_Conservazione_delle_Basi]] — Isomorfismi (Def. 20.4) e conservazione delle basi *(L20)*
- [[157_Teorema_20_5_Teorema_di_Isomorfismo_tra_Spazi_Finitamente_Generati]] — Teorema 20.5 (isomorfismo tra spazi fin. generati) *(L20)*
- [[158_Mappa_delle_Coordinate_e_Mappa_di_Parametrizzazione_Definizione_20_6]] — Mappa delle coordinate e di parametrizzazione (Def. 20.6) *(L20)*
- [[159_Esempio_Mappa_di_Parametrizzazione_Polinomi_di_Grado_al_piu_2]] — Esempio: parametrizzazione di $\mathbb{K}[t]_{\le2}$ *(L20)*
- [[160_Paradigma_Rappresentare_una_Applicazione_Lineare_con_una_Matrice]] — Paradigma: rappresentare $L$ con una matrice *(L20)*

## Note collegate
- [[01_Indice_Lezione_0]]
- [[02_Indice_Lezione_1]]
- [[03_Indice_Lezione_2]]
- [[04_Indice_Lezione_3]]
- [[05_Indice_Lezione_4]]
- [[07_Indice_Lezione_6]]
- [[08_Indice_Lezione_7]]
- [[10_Indice_Lezione_9]]
- [[11_Indice_Lezione_10]]
- [[12_Indice_Lezione_11]]
- [[14_Indice_Lezione_13]]
- [[16_Indice_Lezione_15]]
- [[17_Indice_Lezione_16]]
- [[18_Indice_Lezione_17]]
- [[20_Indice_Lezione_19]]
- [[21_Indice_Lezione_20]]

#GAL/moc
