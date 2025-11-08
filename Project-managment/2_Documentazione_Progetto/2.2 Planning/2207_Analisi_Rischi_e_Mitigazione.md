# 2207 — Analisi Rischi e Mitigazione — Ziradò

Documento allineato a POS (2101), WBS (2202), Gantt (2203) e budget (2205). Obiettivo: identificare, valutare e gestire minacce che possono compromettere tempistiche, scope, qualità o ritorno dell’iniziativa.

## Metodologia
- **Scala probabilità/impatti (1–5):** 1 = irrilevante, 5 = evento quasi certo o blocco grave.
- **Priorità = P × I.** Soglie: 15‑25 (alto, rosso), 8‑14 (medio, arancione), ≤7 (basso, verde).
- **Strategie:** M = Mitigate, A = Avoid, T = Transfer, Acc = Accept. Ogni rischio ha trigger di monitoraggio e contromisure legate ai deliverable WBS.
- **Cadenza:** revisione settimanale durante gli sprint; rivalutazione formale a ogni milestone di release (R1/R2/R3) come da 2203.

## Matrice qualitativa
| Impatto ↓ / Probabilità → | 1 | 2 | 3 | 4 | 5 |
|---|---|---|---|---|---|
| **5 — Critico** | 5 | 10 | 15 | 20 | 25 |
| **4 — Alto** | 4 | 8 | 12 | 16 | 20 |
| **3 — Medio** | 3 | 6 | 9 | 12 | 15 |
| **2 — Basso** | 2 | 4 | 6 | 8 | 10 |
| **1 — Trascurabile** | 1 | 2 | 3 | 4 | 5 |

## Registro rischi
| ID | Descrizione | Categoria | P | I | Priorità | Strategia | Trigger (KRI) | Owner | Mitigazione (azioni preventive) | Contingenza | Residuo | Stato |
|---|---|---|---|---|---|---|---|---|---|---|---|---|
| **RSK‑001** | Bassa adozione utenti nel primo trimestre post‑lancio | Business/Market | 3 | 4 | **12** | M | MAU <60% target POS o rating <4 | Alex | Piano social WBS.7.3.*, referral esercenti, beta con 50 utenti pilota | Incrementare budget ADV (2205), campagna refer-a-friend | Medio | Aperto |
| **RSK‑002** | Contenuti non aggiornati o insufficienti (<30 eventi/mese) | Operativo | 3 | 4 | **12** | M | Contenuti calendarizzati <75% settimana | Alice | Onboarding esercenti (workshop mensile), automatizzare reminder via WBS.6.1.4 | Attivare scraping manuale e promuovere eventi sponsor | Medio | Aperto |
| **RSK‑003** | Ritardi review store (Apple/Google) oltre 7 giorni | Esterno | 2 | 5 | **10** | A | Status “In review” > 7 gg | Alice | Checklist store WBS.7.1.*, build testflight interna, submission anticipata di 2 sett | Richiedere expedited review o spostare finestra campagna | Basso | Aperto |
| **RSK‑004** | Non conformità GDPR (consensi/Privacy Policy) | Compliance | 2 | 5 | **10** | M | Audit checklist WBS.8.3.1 incompleta | Alex | Data minimization, log consenso per evento, revisione legale template | Disattivare feature incriminata e inviare comunicazione utenti | Basso | Aperto |
| **RSK‑005** | Sovraccarico team e slittamento CP R1 | Project Mgmt | 3 | 3 | **9** | M | Burn-down devia >20% o task CP fuori sprint | Alex | WIP limit, retro pianificate, buffer 3 sett in Gantt (2203) | Ridurre scope sprint (es. filtri avanzati) | Medio | Aperto |
| **RSK‑006** | Superamento costi vivi (store, hosting, ADV) rispetto a 404 € | Finanziario | 2 | 3 | **6** | Acc | Spesa >110% budget mensile | Alice | Monitor spese mensili, uso tier gratuito mappe, sponsorship per coprire ADV | Rinviare campagne o passare a infrastrutture free | Basso | Aperto |
| **RSK‑007** | Performance/crash fuori KPI (load >2s o crash >1%) | Tecnico | 2 | 4 | **8** | M | Report Firebase > target per 2 settimane | Alice | Test WBS.8.1–8.2, profiling early, gating tramite beta interna | Rollback build e hotfix bug critici | Basso | Aperto |
| **RSK‑008** | Sponsor/comune non confermano supporto | Stakeholder | 3 | 3 | **9** | M | <3 sponsor confermati entro sprint 8 | Alex | Pipeline sponsor già da WBS.7.2.*, demo personalizzate | Ridurre spesa ADV e aumentare promo organica | Medio | Aperto |
| **RSK‑009** | Dipendenza da API mappe e possibili costi extra | Tecnologico | 2 | 4 | **8** | T | Utilizzo quota >80% mese | Alice | Cache tile, limiti richiesta, valutare fallback OpenStreetMap | Passare temporaneamente a layer statici | Basso | Aperto |
| **RSK‑010** | Recensioni abusive o diffamatorie in R3 | Prod./Qualità | 3 | 3 | **9** | M | >5 segnalazioni inevase/sett | Alice | Moderazione WBS.4.3.*, policy utenti, soglie auto-hide | Sospendere recensioni e comunicare motivazione | Medio | Pianificato |

Legenda strategia: M = Mitigare, A = Evitare, T = Trasferire, Acc = Accettare.

## Piani di risposta (focus rischi prioritari)
- **RSK‑001 / RSK‑002 – Adozione & contenuti:** agganciate al piano marketing (WBS.7.3) e alle notifiche (WBS.6.1.4). Ogni sprint di R1 include KRI su numero eventi caricati e lead esercenti.
- **RSK‑003 – Store review:** buffer di 3 settimane tra fine sviluppo e Go-Live (2203). Asset store e policy vengono congelati in Sprint 9 per ridurre richieste correttive.
- **RSK‑004 – GDPR:** la check-list privacy viene completata prima della submission di ogni release; i log di consenso sono parte del Definition of Done delle user story di autenticazione.
- **RSK‑005 – Capacità team:** uso di Kanban WIP=2 per persona; se il carico supera il limite, il PM rinvia feature non critiche (es. filtri avanzati, slot sponsor aggiuntivi).
- **RSK‑008 – Sponsor:** pipeline con stato (lead → proposta → firma) tracciata in Issues Log (41_Issues_Log_Gestione_Rischi.md). KRI = numero slot venduti vs. target budget (2205).
- **RSK‑010 – Moderazione:** in R3 viene attivata una coda manuale con SLA 48h; le notifiche (WBS.6.3.1) riducono il rischio reputazionale perché informano utenti e gestori sullo stato della segnalazione.

## Monitoraggio e reporting
- **Riunione rischi settimanale** (15’ in ogni sprint review) per aggiornare stato, trigger e azioni.
- **Heatmap aggiornata** nel tool di tracking: un rischio passa a “Chiuso” quando il trigger rimane sotto soglia per 4 settimane o la mitigazione diventa parte del processo standard.
- **Integrazione con Gantt:** gli eventi RSK‑003, RSK‑005 e RSK‑007 sono direttamente collegati alle milestone critiche del CP (2203). Ogni slittamento >2 gg viene riportato nel log modifiche del piano.
- **Collegamento a KPI POS:** break-even (2205) e target MAU rating sono monitorati insieme ai rischi RSK‑001 e RSK‑008 per decidere eventuali pivot post‑R3.
