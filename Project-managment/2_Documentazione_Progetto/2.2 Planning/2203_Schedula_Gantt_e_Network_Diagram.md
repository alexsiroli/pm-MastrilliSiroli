# 2203 — Schedula Gantt e Network Diagram — Ziradò

# Release 1 — Core Experience (R1)

**Calendario**: lun–ven. **Festività ignorate**: 2025-12-24→2026-01-07 e 2026-04-01→2026-04-08. **Start**: 2025-12-01.

TODO Cambiare le date in italiano e la priam data del primo vero task è il 1/12. il 1.2.4 (controllo accesibilita) va tolto da qui, wbs e sitma,
fai in modo che l'ordine dell'esecuziuone dei task wbs siano coerenti con il loro numero di wbs ma il rbs.7.2 e il rbs.7.3 devono essere fatti alla fine della release 1

| **Task id** | **Task description**                                                   | **Effort (person-days)** | **Resources allocated** | **Predecessor** | **Start date** | **Finish date** |
| ----------: | ---------------------------------------------------------------------- | -----------------------: | ----------------------- | --------------- | -------------: | --------------: |
|           1 | Start                                                          |                        0 | —                       |                 |     2025-12-01 |      2025-12-01 |
|           2 | WBS.1.1.1 — Creazione modello dati scheda locale                       |                        3 | Alice                   | 1               |     2025-12-02 |      2025-12-04 |
|           3 | WBS.1.1.2 — Raccolta informazioni di ogni locale                       |                        7 | Alex                    | 1               |     2025-12-02 |      2025-12-10 |
|           4 | WBS.1.1.4 — Sviluppo azioni rapide (call, mappa, share)                |                        5 | Alex                    | 3               |     2025-12-11 |      2025-12-17 |
|           5 | WBS.1.2.1 — Progettazione e sviluppo mappa interattiva                 |                       10 | Alice                   | 2               |     2025-12-05 |      2025-12-18 |
|           6 | WBS.1.3.1 — Definizione e caricamento tipologie locali                 |                        4 | Alice                   | 5               |     2025-12-19 |      2026-01-08 |
|           7 | WBS.2.1.1 — Creazione modello dati evento                              |                        3 | Alice                   | 6               |     2026-01-09 |      2026-01-13 |
|           8 | WBS.5.1.1 — Sviluppo Login/Registrazione                               |                        5 | Alice                   | 7               |     2026-01-14 |      2026-01-20 |
|           9 | WBS.5.1.2 — Gestione interfacce coerenti con il ruolo                  |                        4 | Alex                    | 4               |     2025-12-18 |      2025-12-23 |
|          10 | WBS.5.2.1 — Sviluppo portale admin                                     |                        7 | Alice                   | 8               |     2026-01-21 |      2026-01-29 |
|          11 | WBS.6.1.1 — Sviluppo di un sistema di notifiche                        |                        6 | Alice                   | 10              |     2026-01-30 |      2026-02-06 |
|          12 | WBS.7.1.1 — Preparazione asset store (descrizioni, screenshot, policy) |                        5 | Alex                    | 9               |     2026-01-08 |      2026-01-14 |
|          13 | WBS.7.1.2 — Caricamento e pubblicazione finale sugli store             |                        6 | Alice                   | 11              |     2026-02-09 |      2026-02-16 |
|          14 | WBS.7.2.1 — Progettazione sezione sponsor/advertising                  |                        5 | Alex                    | 12              |     2026-01-15 |      2026-01-21 |
|          15 | WBS.7.2.2 — Implementazione componenti advertising                     |                        8 | Alice                   | 13              |     2026-02-17 |      2026-02-26 |
|          16 | WBS.7.3.1 — Creazione canali social e brand identity                   |                        4 | Alex                    | 14              |     2026-01-22 |      2026-01-27 |
|          17 | WBS.7.3.2 — Piano editoriale e produzione contenuti                    |                        7 | Alice                   | 15              |     2026-02-27 |      2026-03-09 |
|          18 | WBS.8.1.1 — Performance test                                           |                        4 | Alice                   | 17              |     2026-03-10 |      2026-03-13 |
|          19 | WBS.8.2.1 — Monitoraggio crash                                         |                        4 | Alice                   | 18              |     2026-03-16 |      2026-03-19 |
|          20 | WBS.8.3.1 — Valutazione GDPR e consensi                                |                        4 | Alex                    | 16              |     2026-01-28 |      2026-02-02 |
|          21 | WBS.8.4.1 — Conformità store                                           |                        4 | Alex                    | 20              |     2026-02-03 |      2026-02-06 |
|          22 | WBS.8.5.1 — Rispetto accessibilità base                                |                        4 | Alex                    | 21              |     2026-02-09 |      2026-02-12 |
|          23 | WBS.1.1.3 — Sviluppo operazioni CRUD del locale                        |                        7 | Alice                   | 2, 19           |     2026-03-20 |      2026-03-30 |
|          24 | WBS.1.2.2 — Raccolta coordinate geografiche dai locali                 |                        2 | Alex                    | 3, 22           |     2026-02-13 |      2026-02-16 |
|          25 | WBS.2.2.1 — Sviluppo operazioni CRUD su eventi                         |                        7 | Alice                   | 7, 23           |     2026-03-31 |      2026-04-16 |
|          26 | WBS.2.3.1 — Sviluppo di un calendario con eventi                       |                        8 | Alice                   | 7, 25           |     2026-04-17 |      2026-04-28 |
|          27 | WBS.2.3.2 — Sviluppo di una lista di eventi                            |                        4 | Alice                   | 7, 26           |     2026-04-29 |      2026-05-04 |
|          28 | WBS.2.3.3 — Sistema di filtraggio degli eventi                         |                        6 | Alex                    | 6, 7, 24        |     2026-02-17 |      2026-02-24 |
|          29 | WBS.6.1.2 — Gestione trigger clienti                                   |                        4 | Alice                   | 11, 27          |     2026-05-05 |      2026-05-08 |
|          30 | WBS.6.1.4 — Trigger automatici                                         |                        1 | Alice                   | 11, 29          |     2026-05-11 |      2026-05-11 |
|          31 | WBS.7.3.3 — Scheduling pubblicazioni e gestione community              |                        5 | Alex                    | 16, 28          |     2026-02-25 |      2026-03-03 |
|          32 | WBS.1.2.3 — Caricamento locali come punti in mappa                     |                        7 | Alex                    | 24, 31          |     2026-03-04 |      2026-03-12 |
|          33 | WBS.2.2.2 — Validazioni form di creazione/modifica evento              |                        4 | Alex                    | 25, 32          |     2026-04-17 |      2026-04-22 |
|          34 | WBS.6.1.3 — Interfaccia per scegliere le notifiche                     |                        3 | Alex                    | 29, 33          |     2026-05-11 |      2026-05-13 |
|          35 | WBS.1.2.4 — Controllo principi di accessibilità                        |                        4 | Alex                    | 32, 34          |     2026-05-14 |      2026-05-19 |
|          36 | WBS.1.3.2 — Sviluppo sistema filtraggio locali                         |                        6 | Alex                    | 6, 32, 35       |     2026-05-20 |      2026-05-27 |
|          37 | Finish — Finish                                                        |                        0 | —                       | 36              |     2026-05-27 |      2026-05-27 |

# Release 2 — Coupon/Offerte (R2)

**Calendario**: lun–ven. **Start**: 2026-08-01.

| **Task id** | **Task description**                                          | **Effort (person-days)** | **Resources allocated** | **Predecessor** | **Start date** | **Finish date** |
| ----------: | ------------------------------------------------------------- | -----------------------: | ----------------------- | --------------- | -------------: | --------------: |
|           1 | Start — Start                                                 |                        0 | —                       |                 |     2026-08-01 |      2026-08-01 |
|           2 | WBS.3.1.1 — Creazione modello dati coupon                     |                        3 | Alice                   | 1               |     2026-08-03 |      2026-08-05 |
|           3 | WBS.6.2.1 — Trigger notifica clienti su nuovi coupon          |                        4 | Alice                   | 2               |     2026-08-06 |      2026-08-11 |
|           4 | WBS.6.2.2 — Preferenze notifiche coupon in app cliente        |                        3 | Alex                    | 1               |     2026-08-03 |      2026-08-05 |
|           5 | WBS.7.4.2 (R2) — Comunicazione release note e annuncio social |                        3 | Alex                    | 4               |     2026-08-06 |      2026-08-10 |
|           6 | WBS.8.6.1 (R2) — Regression performance/stabilità post-R2     |                        3 | Alice                   | 3               |     2026-08-12 |      2026-08-14 |
|           7 | WBS.8.6.2 (R2) — Verifica privacy/compliance store post-R2    |                        2 | Alex                    | 5               |     2026-08-11 |      2026-08-12 |
|           8 | WBS.3.1.2 — Sviluppo operazioni CRUD per coupon               |                        7 | Alice                   | 2, 6            |     2026-08-17 |      2026-08-25 |
|           9 | WBS.3.2.1 — Interfaccia clienti per visualizzare i coupon     |                        6 | Alex                    | 7, 8            |     2026-08-26 |      2026-09-02 |
|          10 | WBS.3.2.2 — Sistema per utilizzare i coupon                   |                        7 | Alex                    | 9               |     2026-09-03 |      2026-09-11 |
|          11 | WBS.7.4.1 (R2) — Submission aggiornamento R2 sugli store      |                        3 | Alice                   | 8, 10           |     2026-09-14 |      2026-09-16 |
|          12 | Finish — Finish                                               |                        0 | —                       | 11              |     2026-09-16 |      2026-09-16 |

# Release 3 — Recensioni & Moderazione (R3)

**Calendario**: lun–ven. **Start**: 2026-10-15.

| **Task id** | **Task description**                                                               | **Effort (person-days)** | **Resources allocated** | **Predecessor** | **Start date** | **Finish date** |
| ----------: | ---------------------------------------------------------------------------------- | -----------------------: | ----------------------- | --------------- | -------------: | --------------: |
|           1 | Start — Start                                                                      |                        0 | —                       |                 |     2026-10-15 |      2026-10-15 |
|           2 | WBS.4.1.1 — Definizione dei punti di valutazione                                   |                        3 | Alex                    | 1               |     2026-10-16 |      2026-10-20 |
|           3 | WBS.6.3.1 — Notifiche clienti su nuove recensioni/risposte e segnalazioni moderate |                        4 | Alice                   | 1               |     2026-10-16 |      2026-10-21 |
|           4 | WBS.4.1.2 — Sistema per valutare il locale in base ai punti                        |                        7 | Alice                   | 3               |     2026-10-22 |      2026-10-30 |
|           5 | WBS.4.1.3 — Analisi dei punteggi per locale                                        |                        6 | Alex                    | 2               |     2026-10-21 |      2026-10-28 |
|           6 | WBS.4.1.4 — Interfaccia per visualizzare valutazioni a punti                       |                        3 | Alex                    | 4, 5            |     2026-10-29 |      2026-11-02 |
|           7 | WBS.4.2.1 — Creazione modello dati recensione                                      |                        3 | Alice                   | 4               |     2026-11-02 |      2026-11-04 |
|           8 | WBS.4.2.2 — Interfaccia per recensire un locale                                    |                        3 | Alex                    | 7, 6            |     2026-11-03 |      2026-11-05 |
|           9 | WBS.4.2.3 — Interfaccia per visualizzare recensioni testuali                       |                        3 | Alex                    | 8               |     2026-11-06 |      2026-11-10 |
|          10 | WBS.4.3.1 — Sistema per segnalare/gestire recensioni inappropriate                 |                        7 | Alice                   | 7               |     2026-11-05 |      2026-11-13 |
|          11 | WBS.4.3.2 — Interfaccia per segnalare recensioni                                   |                        3 | Alex                    | 10, 9           |     2026-11-11 |      2026-11-13 |
|          12 | WBS.4.3.3 — Interfaccia admin per gestire le segnalazioni                          |                        3 | Alex                    | 10, 11          |     2026-11-16 |      2026-11-18 |
|          13 | WBS.8.6.1 (R3) — Regression performance/stabilità post-R3                          |                        3 | Alice                   | 10              |     2026-11-16 |      2026-11-18 |
|          14 | WBS.7.4.1 (R3) — Submission aggiornamento R3 sugli store                           |                        3 | Alice                   | 12, 13          |     2026-11-19 |      2026-11-23 |
|          15 | WBS.7.4.2 (R3) — Comunicazione release note e annuncio social                      |                        3 | Alex                    | 12              |     2026-11-19 |      2026-11-23 |
|          16 | WBS.8.6.2 (R3) — Verifica privacy/compliance store post-R3                         |                        2 | Alex                    | 15              |     2026-11-24 |      2026-11-25 |
|          17 | Finish — Finish                                                                    |                        0 | —                       | 14              |     2026-12-01 |      2026-12-01 |

