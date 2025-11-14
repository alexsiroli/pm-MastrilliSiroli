# 2204 — Stime e Fabbisogno Risorse — Ziradò

## Metodologia di Stima
- **Tecnica:** Three-Point (Optimistic / Most Likely / Pessimistic).  
- **Formula:** E = (O + 4M + P) / 6  
- **Assunzioni:** 20 h/settimana/persona; efficienza 75% → **15 h/sett = 3 h/giorno effettive**.  
- **Durata effettiva (gg):** E / 3.  
- **Unità:** ore/uomo (effort) e giorni effettivi (3h/giorno).

### Note
Le stime riflettono un approccio **consensus-based Three-Point**, con efficienza realistica del 75%.  
I valori medi (E) sono stati convertiti in durata effettiva dividendo per 3h/giorno di lavoro reale. 
Nella conversione ore => num.giorni, i giorni sono approssimati per eccesso.
Le attività sono distribuite equamente tra backend (Alice) e frontend/UI (Alex).
Si lavora solo 20h/settimana in quanto studenti, e si è fatta una stima considerando periodi con più disopnibilità e altri con meno disponibilità data la consegna di eventuali esami.
Si assume, inoltre, che le competenze di Alex e Alice, avendo lo stesso background, siano le stesse: la divisione del lavoro viene fatta non sulla base delle skill ma dell'interesse dell'uno o dell'altro.
Si adotta uno sviluppo incrementale per release R1–R3, con revisione periodica delle stime.

---

## Tabella Stime per Attività (Three-Point con Durata Effettiva)

### Release 1 · Core Experience (R1)
Comprende tutte le funzionalità necessarie per il lancio iniziale: mappa, eventi, backend/admin, notifiche e requisiti non funzionali abilitanti.

| ID | Nome Attività | O/M/P (h) | Effort Medio (E) | Durata Effettiva (gg) | Ruolo | Note |
|----|----------------|-----------|------------------|------------------------|-------|------|
| **RBS.1 — Mappa** | | | | | | |
| WBS.1.1.1 | Creazione modello dati scheda locale | 6/8/10 | **8 h** | **3 gg** | Alice | — |
| WBS.1.1.2 | Raccolta informazioni di ogni locale | 16/20/28 | **21 h** | **7 gg** | Alex | Input manuale |
| WBS.1.1.3 | Sviluppo operazioni CRUD del locale | 16/20/24 | **20 h** | **7 gg** | Alice | Dip. da WBS.1.1.1 |
| WBS.1.1.4 | Sviluppo azioni rapide (call, mappa, share) | 10/14/22 | **15 h** | **5 gg** | Alex | — |
| WBS.1.2.1 | Progettazione e sviluppo mappa interattiva | 20/28/36 | **28 h** | **10 gg** | Alice | — |
| WBS.1.2.2 | Raccolta coordinate geografiche dai locali | 4/6/8 | **6 h** | **2 gg** | Alex | Dip. da WBS.1.1.2 |
| WBS.1.2.3 | Caricamento locali come punti in mappa | 16/20/28 | **21 h** | **7 gg** | Alex | Dip. da WBS.1.2.2 |
| WBS.1.3.1 | Definizione e caricamento tipologie locali | 8/10/12 | **10 h** | **4 gg** | Alice | — |
| WBS.1.3.2 | Sviluppo sistema filtraggio locali | 12/16/20 | **16 h** | **6 gg** | Alex | Dip. da WBS.1.3.1 e WBS.1.2.3 |
| **Totale RBS.1** | | | **145 h** | **51 gg** | | Alice: 66h (24 gg), Alex: 79h (27 gg) |
| **RBS.2 — Eventi** | | | | | | |
| WBS.2.1.1 | Creazione modello dati evento | 6/8/10 | **8 h** | **3 gg** | Alice | — |
| WBS.2.2.1 | Sviluppo operazioni CRUD su eventi | 16/20/24 | **20 h** | **7 gg** | Alice | Dip. da WBS.2.1.1 |
| WBS.2.2.2 | Validazioni form di creazione/modifica evento | 8/12/16 | **12 h** | **4 gg** | Alex | Dip. da WBS.2.2.1 |
| WBS.2.3.1 | Sviluppo di un calendario con eventi | 16/24/30 | **24 h** | **8 gg** | Alice | Dip. da WBS.2.1.1 |
| WBS.2.3.2 | Sviluppo di una lista di eventi | 8/10/20 | **12 h** | **4 gg** | Alice | Dip. da WBS.2.1.1 |
| WBS.2.3.3 | Sistema di filtraggio degli eventi | 12/16/20 | **16 h** | **6 gg** | Alex | Dip. da WBS.1.3.1 e WBS.2.1.1 |
| **Totale RBS.2** | | | **92 h** | **32 gg** | | Alice: 64h (22 gg), Alex: 28h (10 gg) |
| **RBS.5 — Backend/API e Admin** | | | | | | |
| WBS.5.1.1 | Sviluppo Login/Registrazione | 10/12/18 | **13 h** | **5 gg** | Alice | — |
| WBS.5.1.2 | Gestione interfacce coerenti con il ruolo | 8/12/16 | **12 h** | **4 gg** | Alex | — |
| WBS.5.2.1 | Sviluppo portale admin | 18/20/26 | **21 h** | **7 gg** | Alice | — |
| **Totale RBS.5** | | | **46 h** | **16 gg** | | Alice: 34h (12 gg), Alex: 12h (4 gg) |
| **RBS.6 — Sistema Notifiche** | | | | | | |
| WBS.6.1.1 | Sviluppo di un sistema di notifiche | 16/18/20 | **18 h** | **6 gg** | Alice | — |
| WBS.6.1.2 | Gestione trigger clienti | 8/10/16 | **11 h** | **4 gg** | Alice | Dip. da WBS.6.1.1 |
| WBS.6.1.3 | Interfaccia per scegliere le notifiche | 6/8/12 | **8 h** | **3 gg** | Alex | Dip. da WBS.6.1.2 |
| WBS.6.1.4 | Trigger automatici | 2/3/4 | **3 h** | **1 gg** | Alice | Dip. da WBS.6.1.1 |
| **Totale RBS.6** | | | **40 h** | **14 gg** | | Alice: 32h (11 gg), Alex: 8h (3 gg) |
| **RBS.7 — Attività di lancio e sponsorizzazione** | | | | | | |
| WBS.7.1.1 | Preparazione asset store (descrizioni, screenshot, policy) | 12/15/18 | **15 h** | **5 gg** | Alex | — |
| WBS.7.1.2 | Caricamento e pubblicazione finale sugli store | 12/18/24 | **18 h** | **6 gg** | Alice | — |
| WBS.7.2.1 | Progettazione sezione sponsor/advertising | 10/14/18 | **14 h** | **5 gg** | Alex | Layout card sponsor, banner e CTA. |
| WBS.7.2.2 | Implementazione componenti advertising | 18/24/30 | **24 h** | **8 gg** | Alice | Integrazione API/SDK e analytics. |
| WBS.7.3.1 | Creazione canali social e brand identity | 8/12/16 | **12 h** | **4 gg** | Alex | — |
| WBS.7.3.2 | Piano editoriale e produzione contenuti | 12/18/30 | **19 h** | **7 gg** | Alice | — |
| WBS.7.3.3 | Scheduling pubblicazioni e gestione community | 9/14/19 | **14 h** | **5 gg** | Alex | Dip. da WBS.7.3.1 |
| **Totale RBS.7 (R1)** | | | **116 h** | **40 gg** | | Alice: 61h (21 gg), Alex: 55h (19 gg) |
| **RBS.8 — Requisiti Non Funzionali** | | | | | | |
| WBS.8.1.1 | Performance test | 8/12/16 | **12 h** | **4 gg** | Alice | — |
| WBS.8.2.1 | Monitoraggio crash | 8/12/16 | **12 h** | **4 gg** | Alice | — |
| WBS.8.3.1 | Valutazione GDPR e consensi | 8/12/16 | **12 h** | **4 gg** | Alex | — |
| WBS.8.4.1 | Conformità store | 8/12/16 | **12 h** | **4 gg** | Alex | — |
| WBS.8.5.1 | Rispetto accessibilità base | 8/12/16 | **12 h** | **4 gg** | Alex | — |
| **Totale RBS.8** | | | **60 h** | **20 gg** | | Alice: 24h (8 gg), Alex: 36h (12 gg) |
| **Totale Release 1** | | | **499 h** | **173 gg** | | Alice: 281h (98 gg), Alex: 218h (75 gg) |

### Release 2 · Coupon/Offerte (R2)
Copre il pacchetto funzionale previsto per la seconda release (RBS.3).

| ID | Nome Attività | O/M/P (h) | Effort Medio (E) | Durata Effettiva (gg) | Ruolo | Note |
|----|----------------|-----------|------------------|------------------------|-------|------|
| **RBS.3 — Coupon/Offerte** | | | | | | |
| WBS.3.1.1 | Creazione modello dati coupon | 6/8/10 | **8 h** | **3 gg** | Alice | — |
| WBS.3.1.2 | Sviluppo operazioni CRUD per coupon | 16/20/24 | **20 h** | **7 gg** | Alice | Dip. da WBS.3.1.1 |
| WBS.3.2.1 | Interfaccia clienti per visualizzare i coupon | 12/16/20 | **16 h** | **6 gg** | Alex | Dip. da WBS.3.1.2 |
| WBS.3.2.2 | Sistema per utilizzare i coupon | 16/20/28 | **21 h** | **7 gg** | Alex | Dip. da WBS.3.2.1 |
| **RBS.6 — Sistema Notifiche (R2)** | | | | | | |
| WBS.6.2.1 | Trigger notifica clienti su nuovi coupon | 8/12/16 | **12 h** | **4 gg** | Alice |
| WBS.6.2.2 | Preferenze notifiche coupon in app cliente | 6/8/12 | **8 h** | **3 gg** | Alex | 
| **Totale RBS.6 (R2)** | | | **20 h** | **7 gg** | | Alice: 12h (4 gg), Alex: 8h (3 gg) |
| **RBS.7 — Attività di lancio e sponsorizzazione** | | | | | | Aggiornamento R2 |
| WBS.7.4.1 | Submission aggiornamento R2 sugli store | 6/8/12 | **8 h** | **3 gg** | Alice | Dip. da WBS.3.2.2 |
| WBS.7.4.2 | Comunicazione release note e annuncio social | 6/9/12 | **9 h** | **3 gg** | Alex | Include update sulle community. |
| **Totale RBS.7 (R2)** | | | **17 h** | **6 gg** | | Alice: 8h (3 gg), Alex: 9h (3 gg) |
| **RBS.8 — Requisiti Non Funzionali (Regression R2)** | | | | | | |
| WBS.8.6.1 | Regression performance/stabilità post-R2 | 6/8/12 | **8 h** | **3 gg** | Alice | Test sintetico su viste principali. |
| WBS.8.6.2 | Verifica privacy/compliance store post-R2 | 4/6/8 | **6 h** | **2 gg** | Alex | Checklist GDPR/Store aggiornata. |
| **Totale RBS.8 (R2)** | | | **14 h** | **5 gg** | | Alice: 8h (3 gg), Alex: 6h (2 gg) |
| **Totale Release 2** | | | **116 h** | **41 gg** | | Alice: 56h (20 gg), Alex: 60h (21 gg) |

### Release 3 · Recensioni & Moderazione (R3)
Include l’intero blocco recensioni e moderazione previsto da RBS.4.

| ID | Nome Attività | O/M/P (h) | Effort Medio (E) | Durata Effettiva (gg) | Ruolo | Note |
|----|----------------|-----------|------------------|------------------------|-------|------|
| **RBS.4 — Recensioni** | | | | | | |
| WBS.4.1.1 | Definizione dei punti di valutazione | 4/8/12 | **8 h** | **3 gg** | Alex | Dip. da WBS.1.3.1 |
| WBS.4.1.2 | Sistema per valutare il locale in base ai punti | 14/20/28 | **20 h** | **7 gg** | Alice | — |
| WBS.4.1.3 | Analisi dei punteggi per locale | 12/16/20 | **16 h** | **6 gg** | Alex | Dip. da WBS.4.1.1 |
| WBS.4.1.4 | Interfaccia per visualizzare valutazioni a punti | 6/8/12 | **8 h** | **3 gg** | Alex | Dip. da WBS.4.1.2 |
| WBS.4.2.1 | Creazione modello dati recensione | 6/8/10 | **8 h** | **3 gg** | Alice | — |
| WBS.4.2.2 | Interfaccia per recensire un locale | 6/8/12 | **8 h** | **3 gg** | Alex | Dip. da WBS.4.2.1 |
| WBS.4.2.3 | Interfaccia per visualizzare recensioni testuali | 6/8/12 | **8 h** | **3 gg** | Alex | Dip. da WBS.4.2.1 |
| WBS.4.3.1 | Sistema per segnalare/gestire recensioni inappropriate | 16/20/28 | **21 h** | **7 gg** | Alice | Dip. da WBS.4.2.1 |
| WBS.4.3.2 | Interfaccia per segnalare recensioni | 6/8/12 | **8 h** | **3 gg** | Alex | Dip. da WBS.4.3.1 |
| WBS.4.3.3 | Interfaccia admin per gestire le segnalazioni | 6/8/12 | **8 h** | **3 gg** | Alex | Dip. da WBS.4.3.1 |
| **RBS.6 — Sistema Notifiche (R3)** | | | | | | |
| WBS.6.3.1 | Notifiche clienti su nuove recensioni/risposte e segnalazioni moderate | 8/12/16 | **12 h** | **4 gg** | Alice | 
| **Totale RBS.6 (R3)** | | | **12 h** | **4 gg** | | Alice: 12h (4 gg), Alex: — |
| **RBS.7 — Attività di lancio e sponsorizzazione** | | | | | | Aggiornamento R3 |
| WBS.7.4.1 | Submission aggiornamento R3 sugli store | 6/8/12 | **8 h** | **3 gg** | Alice | Dip. da WBS.4.3.3 |
| WBS.7.4.2 | Comunicazione release note e annuncio social | 6/9/12 | **9 h** | **3 gg** | Alex | — |
| **Totale RBS.7 (R3)** | | | **17 h** | **6 gg** | | Alice: 8h (3 gg), Alex: 9h (3 gg) |
| **RBS.8 — Requisiti Non Funzionali (Regression R3)** | | | | | | |
| WBS.8.6.1 | Regression performance/stabilità post-R3 | 6/8/12 | **8 h** | **3 gg** | Alice | — |
| WBS.8.6.2 | Verifica privacy/compliance store post-R3 | 4/6/8 | **6 h** | **2 gg** | Alex | — |
| **Totale RBS.8 (R3)** | | | **14 h** | **5 gg** | | Alice: 8h (3 gg), Alex: 6h (2 gg) |
| **Totale Release 3** | | | **156 h** | **56 gg** | | Alice: 77h (27 gg), Alex: 79h (29 gg) |

### Totale complessivo progetto

| Release | Ore totali | Giorni effettivi | Alice (h / gg) | Alex (h / gg) |
|---------|------------|------------------|-----------------|----------------|
| R1 | **499 h** | **173 gg** | 281 h / 98 gg | 218 h / 75 gg |
| R2 | **116 h** | **41 gg** | 56 h / 20 gg | 60 h / 21 gg |
| R3 | **156 h** | **56 gg** | 77 h / 27 gg | 79 h / 29 gg |
| **Totale** | **771 h** | **270 gg** | 414 h / 145 gg | 357 h / 125 gg |

## Previsione temporale (sintesi)

Capacità team: 30 h/settimana (15 h/sett per persona). Le durate sotto sono una stima calendario (settimane) ricavate dalle ore totali per release, con tolleranza per dipendenze e sovrapposizioni tra task. I “giorni effettivi” in tabella equivalgono a giornate da 3 ore e non rappresentano giorni di calendario.

- R1 (core): 98 gg effettivi → ≈ 20 settimane (5 mesi)
- R2 (coupon + notifiche e rilascio): 21 gg effettivi → ≈ 4 settimane (1 mese)
- R3 (recensioni + notifiche e rilascio): 29 gg effettivi → ≈ 6 settimane (≈ 1,5 mesi)

Nota: le stime includono le attività di pubblicazione/annuncio (RBS.7.4) e i re‑test non funzionali post‑release (RBS.8.6) per R2 e R3. Le previsioni non tengono in considerazione i periodi di festività di Natale e Pasqua, con il diagramma di Gantt si avranno stime più precise.
