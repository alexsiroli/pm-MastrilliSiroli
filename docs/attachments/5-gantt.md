# 2203 — **Schedula Gantt e Network Diagram — Ziradò**

## **Release 1 — Core Experience (R1)**

**Calendario**: lun–ven. **Festività non lavorative ignorate**: **24/12/2025→07/01/2026** e **01/04/2026→08/04/2026**.
**Start**: **01/12/2025**.

| **Task id** | **Task description**                                                   | **Effort (person-days)** | **Resources allocated** | **Predecessor** | **Start date** | **Finish date** |
| ----------: | ---------------------------------------------------------------------- | -----------------------: | ----------------------- | --------------- | -------------: | --------------: |
|           1 | Start                                                                  |                        0 | —                       |                 | **01/12/2025** |  **01/12/2025** |
|           2 | WBS.1.1.1 — Creazione modello dati scheda locale                       |                        3 | Alice                   | 1               | **01/12/2025** |  **03/12/2025** |
|           3 | WBS.1.1.2 — Raccolta informazioni di ogni locale                       |                        7 | Alex                    | 1               | **01/12/2025** |  **09/12/2025** |
|           4 | WBS.1.1.3 — Sviluppo operazioni CRUD del locale                        |                        7 | Alice                   | 2               | **04/12/2025** |  **12/12/2025** |
|           5 | WBS.1.1.4 — Sviluppo azioni rapide (call, mappa, share)                |                        5 | Alex                    | 3               | **10/12/2025** |  **16/12/2025** |
|           6 | WBS.1.2.1 — Progettazione e sviluppo mappa interattiva                 |                       10 | Alice                   | 4               | **15/12/2025** |  **12/01/2026** |
|           7 | WBS.1.2.2 — Raccolta coordinate geografiche dai locali                 |                        2 | Alex                    | 6, 3            | **13/01/2026** |  **14/01/2026** |
|           8 | WBS.1.2.3 — Caricamento locali come punti in mappa                     |                        7 | Alex                    | 7               | **15/01/2026** |  **23/01/2026** |
|           9 | WBS.1.3.1 — Definizione e caricamento tipologie locali                 |                        4 | Alice                   | 6               | **13/01/2026** |  **16/01/2026** |
|          10 | WBS.1.3.2 — Sviluppo sistema filtraggio locali                         |                        6 | Alex                    | 9, 8            | **26/01/2026** |  **02/02/2026** |
|          11 | WBS.2.1.1 — Creazione modello dati evento                              |                        3 | Alice                   | 9               | **19/01/2026** |  **21/01/2026** |
|          12 | WBS.2.2.1 — Sviluppo operazioni CRUD su eventi                         |                        7 | Alice                   | 11              | **22/01/2026** |  **30/01/2026** |
|          13 | WBS.2.2.2 — Validazioni form di creazione/modifica evento              |                        4 | Alex                    | 12, 8           | **03/02/2026** |  **06/02/2026** |
|          14 | WBS.2.3.1 — Sviluppo di un calendario con eventi                       |                        8 | Alice                   | 13              | **09/02/2026** |  **18/02/2026** |
|          15 | WBS.2.3.2 — Sviluppo di una lista di eventi                            |                        4 | Alice                   | 14              | **19/02/2026** |  **24/02/2026** |
|          16 | WBS.2.3.3 — Sistema di filtraggio degli eventi                         |                        6 | Alex                    | 15, 11, 9       | **25/02/2026** |  **04/03/2026** |
|          17 | WBS.5.1.1 — Sviluppo Login/Registrazione                               |                        5 | Alice                   | 16              | **23/03/2026** |  **30/03/2026** |
|          18 | WBS.5.1.2 — Gestione interfacce coerenti con il ruolo                  |                        4 | Alex                    | 17              | **31/03/2026** |  **13/04/2026** |
|          19 | WBS.5.2.1 — Sviluppo portale admin                                     |                        7 | Alice                   | 17              | **14/04/2026** |  **22/04/2026** |
|          20 | WBS.6.1.1 — Sviluppo di un sistema di notifiche                        |                        6 | Alice                   | 19              | **23/04/2026** |  **30/04/2026** |
|          21 | WBS.6.1.2 — Gestione trigger clienti                                   |                        4 | Alice                   | 20              | **01/05/2026** |  **06/05/2026** |
|          22 | WBS.6.1.3 — Interfaccia per scegliere le notifiche                     |                        3 | Alex                    | 21              | **07/05/2026** |  **11/05/2026** |
|          23 | WBS.6.1.4 — Trigger automatici                                         |                        1 | Alice                   | 21              | **07/05/2026** |  **07/05/2026** |
|          24 | WBS.7.1.1 — Preparazione asset store (descrizioni, screenshot, policy) |                        5 | Alex                    | 22              | **12/05/2026** |  **18/05/2026** |
|          25 | WBS.7.2.1 — Progettazione sezione sponsor/advertising                  |                        5 | Alex                    | 24              | **19/05/2026** |  **25/05/2026** |
|          26 | WBS.7.2.2 — Implementazione componenti advertising                     |                        8 | Alice                   | 25              | **25/05/2026** |  **03/06/2026** |
|          27 | WBS.7.3.1 — Creazione canali social e brand identity                   |                        4 | Alex                    | 26              | **04/06/2026** |  **09/06/2026** |
|          28 | WBS.7.3.2 — Piano editoriale e produzione contenuti                    |                        7 | Alice                   | 27              | **10/06/2026** |  **18/06/2026** |
|          29 | WBS.7.3.3 — Scheduling pubblicazioni e gestione community              |                        5 | Alex                    | 27              | **10/06/2026** |  **16/06/2026** |
|          30 | WBS.8.1.1 — Performance test                                           |                        4 | Alice                   | 29              | **17/06/2026** |  **22/06/2026** |
|          31 | WBS.8.2.1 — Monitoraggio crash                                         |                        4 | Alice                   | 30              | **23/06/2026** |  **26/06/2026** |
|          32 | WBS.8.3.1 — Valutazione GDPR e consensi                                |                        4 | Alex                    | 29              | **17/06/2026** |  **22/06/2026** |
|          33 | WBS.8.4.1 — Conformità store                                           |                        4 | Alex                    | 32              | **23/06/2026** |  **26/06/2026** |
|          34 | WBS.7.1.2 — Caricamento e pubblicazione finale sugli store             |                        6 | Alice                   | 33              | **29/06/2026** |  **06/07/2026** |
|          35 | Finish — Finish                                                        |                        0 | —                       | 34              | **06/07/2026** |  **06/07/2026** |

---

## **Release 2 — Coupon/Offerte (R2)**

**Calendario**: lun–ven. **Start**: **01/08/2026**.

| **Task id** | **Task description**                                          | **Effort (person-days)** | **Resources allocated** | **Predecessor** | **Start date** | **Finish date** |
| ----------: | ------------------------------------------------------------- | -----------------------: | ----------------------- | --------------- | -------------: | --------------: |
|           1 | Start — Start                                                 |                        0 | —                       |                 | **01/08/2026** |  **01/08/2026** |
|           2 | WBS.3.1.1 — Creazione modello dati coupon                     |                        3 | Alice                   | 1               | **01/08/2026** |  **05/08/2026** |
|           3 | WBS.6.2.1 — Trigger notifica clienti su nuovi coupon          |                        4 | Alice                   | 2               | **06/08/2026** |  **11/08/2026** |
|           4 | WBS.6.2.2 — Preferenze notifiche coupon in app cliente        |                        3 | Alex                    | 1               | **01/08/2026** |  **05/08/2026** |
|           5 | WBS.7.4.2 (R2) — Comunicazione release note e annuncio social |                        3 | Alex                    | 4               | **06/08/2026** |  **10/08/2026** |
|           6 | WBS.8.6.1 (R2) — Regression performance/stabilità post-R2     |                        3 | Alice                   | 3               | **12/08/2026** |  **14/08/2026** |
|           7 | WBS.8.6.2 (R2) — Verifica privacy/compliance store post-R2    |                        2 | Alex                    | 5               | **11/08/2026** |  **12/08/2026** |
|           8 | WBS.3.1.2 — Sviluppo operazioni CRUD per coupon               |                        7 | Alice                   | 2, 6            | **17/08/2026** |  **25/08/2026** |
|           9 | WBS.3.2.1 — Interfaccia clienti per visualizzare i coupon     |                        6 | Alex                    | 7, 8            | **26/08/2026** |  **02/09/2026** |
|          10 | WBS.3.2.2 — Sistema per utilizzare i coupon                   |                        7 | Alex                    | 9               | **03/09/2026** |  **11/09/2026** |
|          11 | WBS.7.4.1 (R2) — Submission aggiornamento R2 sugli store      |                        3 | Alice                   | 8, 10           | **14/09/2026** |  **16/09/2026** |
|          12 | Finish — Finish                                               |                        0 | —                       | 11              | **16/09/2026** |  **16/09/2026** |

---

## **Release 3 — Recensioni & Moderazione (R3)**

**Calendario**: lun–ven. **Start**: **15/10/2026**.

| **Task id** | **Task description**                                                               | **Effort (person-days)** | **Resources allocated** | **Predecessor** | **Start date** | **Finish date** |
| ----------: | ---------------------------------------------------------------------------------- | -----------------------: | ----------------------- | --------------- | -------------: | --------------: |
|           1 | Start — Start                                                                      |                        0 | —                       |                 | **15/10/2026** |  **15/10/2026** |
|           2 | WBS.4.1.1 — Definizione dei punti di valutazione                                   |                        3 | Alex                    | 1               | **15/10/2026** |  **20/10/2026** |
|           3 | WBS.6.3.1 — Notifiche clienti su nuove recensioni/risposte e segnalazioni moderate |                        4 | Alice                   | 1               | **15/10/2026** |  **21/10/2026** |
|           4 | WBS.4.1.2 — Sistema per valutare il locale in base ai punti                        |                        7 | Alice                   | 3               | **22/10/2026** |  **30/10/2026** |
|           5 | WBS.4.1.3 — Analisi dei punteggi per locale                                        |                        6 | Alex                    | 2               | **21/10/2026** |  **28/10/2026** |
|           6 | WBS.4.1.4 — Interfaccia per visualizzare valutazioni a punti                       |                        3 | Alex                    | 4, 5            | **29/10/2026** |  **02/11/2026** |
|           7 | WBS.4.2.1 — Creazione modello dati recensione                                      |                        3 | Alice                   | 4               | **02/11/2026** |  **04/11/2026** |
|           8 | WBS.4.2.2 — Interfaccia per recensire un locale                                    |                        3 | Alex                    | 7, 6            | **03/11/2026** |  **05/11/2026** |
|           9 | WBS.4.2.3 — Interfaccia per visualizzare recensioni testuali                       |                        3 | Alex                    | 8               | **06/11/2026** |  **10/11/2026** |
|          10 | WBS.4.3.1 — Sistema per segnalare/gestire recensioni inappropriate                 |                        7 | Alice                   | 7               | **05/11/2026** |  **13/11/2026** |
|          11 | WBS.4.3.2 — Interfaccia per segnalare recensioni                                   |                        3 | Alex                    | 10, 9           | **11/11/2026** |  **13/11/2026** |
|          12 | WBS.4.3.3 — Interfaccia admin per gestire le segnalazioni                          |                        3 | Alex                    | 10, 11          | **16/11/2026** |  **18/11/2026** |
|          13 | WBS.8.6.1 (R3) — Regression performance/stabilità post-R3                          |                        3 | Alice                   | 10              | **16/11/2026** |  **18/11/2026** |
|          14 | WBS.7.4.2 (R3) — Comunicazione release note e annuncio social                      |                        3 | Alex                    | 12              | **19/11/2026** |  **23/11/2026** |
|          15 | WBS.8.6.2 (R3) — Verifica privacy/compliance store post-R3                         |                        2 | Alex                    | 14              | **24/11/2026** |  **25/11/2026** |
|          16 | WBS.7.4.1 (R3) — Submission aggiornamento R3 sugli store                           |                        3 | Alice                   | 15      | **26/11/2026** |  **30/11/2026** |
|          17 | Finish — Finish                                                                    |                        0 | —                       | 16              | **01/12/2026** |  **01/12/2026** |
