---
layout: page
title: Ziradò
permalink: /attachments/6-analisi-costi/
---

# **Analisi Costi e Budget**

## Scopo e allineamento
- Riferimento a [1-pos.md – Project Overview Statement (POS)]({{ '/attachments/1-pos/' | relative_url }}): break-even entro 12 mesi tramite sponsorship/advertising e vincolo di budget iniziale minimo.
- Coerenza con [2-rbs.md – Requirements Breakdown Structure (RBS)]({{ '/attachments/2-rbs/' | relative_url }}) e [4-wbs.md – Work Breakdown Structure (WBS)]({{ '/attachments/4-wbs/' | relative_url }}): le voci di costo seguono i pacchetti di lavoro effettivamente stimati in [5-stime-e-fabbisogno.md – Stime e Fabbisogno Risorse]({{ '/attachments/5-stime-e-fabbisogno/' | relative_url }}).
- Campo di applicazione: Release R1–R3 previste nel piano (core experience, coupon, recensioni) e attività di lancio/aggiornamento.

## Assunzioni economiche
- Team: Alice (backend/admin) e Alex (frontend/growth); nessun compenso diretto ma valorizziamo le ore per valutare sostenibilità.
- Metodo di stima: Three-Point (O/M/P) con conversione 15 h/settimana/persona, come da [5-stime-e-fabbisogno.md – Stime e Fabbisogno Risorse]({{ '/attachments/5-stime-e-fabbisogno/' | relative_url }}).
- Tariffa di valorizzazione: 25 €/h (benchmark freelance entry-level in ambito mobile).
- Periodo considerato: sviluppo delle tre release + 12 mesi di esercizio per coprire hosting e dominio.

## Struttura dei costi
- **Costi diretti:** uscite di cassa necessarie per abilitare pubblicazione e infrastruttura (licenze store, dominio, hosting, budget marketing).
- **Valorizzazione manodopera:** ore dei founder convertite in euro per avere un riferimento economico e per definire la soglia di successo (anche se non fatturate). 783 h complessive → 19.575 € di lavoro founder.
- **Riserve/contingenza:** cuscinetto del 10% per assorbire slittamenti su attività di marketing, moderazione o infrastruttura.

### Costi diretti
| Voce | WBS / Deliverable | Quantità | Costo (€) | Note e allocazione |
| --- | --- | --- | --- | --- |
| Apple Developer Program | WBS.7.1 / submission store | 1 canone annuo | **94** | Attiva R1 ma abilita anche R2–R3. |
| Google Play Console | WBS.7.1 | Una tantum | **25** | Pagato una sola volta prima del lancio R1. |
| Dominio + DNS | WBS.7.3 | 1 canone annuo  | **15** | zirado.it con gestione DNS. |
| Hosting Firebase con mappe | RBS.1, RBS.5 | 10 €/mese × 12 mesi | **120** | Include DB, storage asset e mappe. |
| Budget contenuti e ADV | RBS.7.3 | 50 €/mese × 3 mesi | **150** | Promozione social per lancio e due update. |
| **Totale costi diretti** |  |  | **404** |

### Valorizzazione manodopera founder
> Ore totali dal file Stime_e_Fabbisogno_Risorse. Il valore non viene pagato ma rappresenta l'investimento di tempo che dovremmo recuperare per considerarci "in pari".

#### Sintesi per release
| Release | Ore Alice | Ore Alex | Ore totali | Valore 25 €/h |
| --- | --- | --- | --- | --- |
| R1 – Core | 281 h | 230 h | **511 h** | **12.775 €** |
| R2 – Coupon | 56 h | 60 h | **116 h** | **2.900 €** | 
| R3 – Recensioni | 77 h | 79 h | **156 h** | **3.900 €** |
| **Totale** | **414 h** | **369 h** | **783 h** | **19.575 €** |

## Budget complessivo e riserve
| Voce | Importo (€) |
| --- | --- |
| Valorizzazione manodopera founder | **19.575** | 
| Costi diretti | **404** | 
| Riserve (10% manodopera) | **1.958** | 
| **Totale costi** | **21.967** | 

## Soglie di successo economico
- **Break-even di cassa (POS):** bastano ~500 € di ricavi sponsorship/ADV entro 6 mesi per coprire i costi diretti, in linea con il criterio del POS.
- **Break-even valorizzato:** includendo il valore del nostro tempo il progetto "va in pari" dopo 19.575 € di ricavi (21.967 € considerando le riserve). Questa è la soglia che usiamo per valutare se l'iniziativa ripaga il tempo investito dagli startupper.
- **Monitoraggio per release:** R1 assorbe il 65% del valore del progetto (12.775 €). Ogni rilascio successivo deve portare almeno 3.000 € di entrate nette cumulative per giustificare l'evoluzione funzionale.
