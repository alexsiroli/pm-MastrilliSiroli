# 2204 — Stime e Fabbisogno Risorse — Ziradò

**Scopo:** stimare effort, durata e definire il fabbisogno di risorse per l’intero progetto *Ziradò*, sulla base del WBS approvato.

---

## Metodologia di Stima
- **Tecnica:** Three-Point (Optimistic / Most Likely / Pessimistic).  
- **Formula:** E = (O + 4M + P) / 6  
- **Assunzioni:** 20 h/settimana/persona; efficienza 75% → **15 h/sett = 3 h/giorno effettive**.  
- **Durata effettiva (gg):** E / 3.  
- **Rischio:** buffer del 10% applicato sul Critical Path.  
- **Unità:** ore/uomo (effort) e giorni effettivi (3h/giorno).

### Note
Le stime riflettono un approccio **consensus-based Three-Point**, con efficienza realistica del 75%.  
I valori medi (E) sono stati convertiti in durata effettiva dividendo per 3h/giorno di lavoro reale. 
Nella conversione ore => num.giorni, i giorni sono approssimati per eccesso.
Le attività sono distribuite equamente tra backend (Alice) e frontend/UI (Alex).
Si lavora solo 20h/settimana in quanto studenti, e si è fatta una stima considerando periodi con meno disponibilità data la consegna di esami e periodi con più disponibilità.
Si assume, inoltre, che le competenze di Alex e Alice, avendo lo stesso background, siano le stesse: la divisione del lavoro viene fatta non sulla base delle skill ma dell'interesse dell'uno o dell'altro.
Si adotta uno sviluppo incrementale per release R1–R3, con revisione periodica delle stime e buffer di 10% applicato alle attività critiche (mappe, notifiche, CRUD locali).

---

## Tabella Stime per Attività (Three-Point con Durata Effettiva)

| ID | Nome Attività | O/M/P (h) | Effort Medio (E) | Durata Effettiva (gg) | Ruolo | Note |
|----|----------------|------------|------------------|------------------------|--------|------|
| **RBS.1 — Mappa** | | | | | | |
| WBS.1.1.1 | Creazione modello dati scheda locale | 6/8/10 | **8 h** | **3 gg** | Alice | — |
| WBS.1.1.2 | Raccolta informazioni di ogni locale | 16/20/28 | **21 h** | **7 gg** | Alex | Input manuale |
| WBS.1.1.3 | Sviluppo operazioni CRUD del locale | 16/20/24 | **20 h** | **7 gg** | Alice | Dip. da WBS.1.1.1 |
| WBS.1.1.4 | Sviluppo azioni rapide (call, mappa, share) | 10/14/22 | **15 h** | **5 gg** | Alex | — |
| WBS.1.2.1 | Progettazione e sviluppo mappa interattiva | 20/28/36 | **28 h** | **10 gg** | Alice | — |
| WBS.1.2.2 | Raccolta coordinate geografiche dai locali | 4/6/8 | **6 h** | **2 gg** | Alex | Dip. da WBS.1.1.2 |
| WBS.1.2.3 | Caricamento locali come punti in mappa | 16/20/28 | **21 h** | **7 gg** | Alex | Dip. da WBS.1.2.2 |
| WBS.1.2.4 | Controllo principi di accessibilità | 8/12/16 | **12 h** | **4 gg** | Alex | Dip. da WBS.1.2.3 |
| WBS.1.3.1 | Definizione e caricamento tipologie locali | 8/10/12 | **10 h** | **4 gg** | Alice | — |
| WBS.1.3.2 | Sviluppo sistema filtraggio locali | 12/16/20 | **16 h** | **6 gg** | Alex | Dip. da WBS.1.3.1 e WBS.1.2.3 |
| **Totale RBS.1** | | | **157 h** | **55 gg** | |Alice: 66h (24 gg), Alex: 91h (31 gg) |
| **RBS.2 — Eventi** | | | | | | |
| WBS.2.1.1 | Creazione modello dati evento | 6/8/10 | **8 h** | **3 gg** | Alice | — |
| WBS.2.2.1 | Sviluppo operazioni CRUD su eventi | 16/20/24 | **20 h** | **7 gg** | Alice | Dip. da WBS.2.1.1 |
| WBS.2.2.2 | Sviluppo di sistema di validazione form creazione/modifica evento | 8/12/16 | **12h** | **4gg** | Alex | Dip. da WBS.2.2.1 |
| WBS.2.3.1 | Sviluppo di un calendario con eventi | 16/24/30 | **24h** | **8gg** | Alice | Dip. da WBS.2.1.1 |
| WBS.2.3.2 | Sviluppo di una lista di eventi | 8/10/20 | **12h** | **4gg** |Alice | Dip. da WBS.2.1.1 |
| WBS.2.3.3 | Sviluppo di un sistema di filtraggio degli eventi  | 12/16/20 | **16 h** | **6 gg** | Alex | Dip. da WBS.1.3.1 e WBS.2.1.1 |
| **Totale RBS.2** | | | **92 h** | **32 gg** | |Alice: 64h (22gg), Alex: 28h (10gg) |
| **RBS.3 — Coupon/Offerte** | | | | | | |
| WBS.3.1.1 | Creazione modello dati coupon | 6/8/10 | **8 h** | **3 gg** | Alice | — |
| WBS.3.1.2 | Sviluppo operazioni CRUD per coupon | 16/20/24 | **20 h** | **7 gg** | Alice | Dip. da WBS.3.1.1 |
| WBS.3.2.1 | Sviluppo dell'interfaccia clienti per visualizzare i coupon | 12/16/20 | **16h** | **6gg** | Alex | Dip. da WBS.3.1.2 |
| WBS.3.2.2 | Sviluppo di un sistema per utilizzare i coupon | 16/20/28 | **21h** | **7gg** | Alex | Dip. da WBS.3.2.1 |
| **Totale RBS.3** | | | **65 h** | **23 gg** | |Alice: 28h (10gg), Alex:37h (13gg) |
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
| **Totale RBS.4** | | | **113 h** | **41 gg** | | Alice: **49 h (17 gg)**, Alex: **64 h (24 gg)** |
| **RBS.5 — Backend/API e Admin** | | | | | | |
| WBS.5.1.1 | Sviluppo Login/Registrazione | 10/12/18 | **13 h** | **5 gg** | Alice | — |
| WBS.5.1.2 | Gestione interfacce coerenti con il ruolo | 8/12/16 | **12 h** | **4 gg** | Alex | — |
| WBS.5.2.1 | Sviluppo portale admin | 18/20/26 | **21 h** | **7 gg** | Alice | — |
| **Totale RBS.5** | | | **46 h** | **16 gg** | | Alice: **34 h (12 gg)**, Alex: **12 h (4 gg)** |
| **RBS.6 — Sistema Notifiche** | | | | | | |
| WBS.6.1.1 | Sviluppo di un sistema di notifiche | 16/18/20 | **18 h** | **6 gg** | Alice | — |
| WBS.6.1.2 | Gestione Trigger clienti | 8/10/16 | **11 h** | **4 gg** | Alice | Dip. da WBS.6.1.1 |
| WBS.6.1.3 | Sviluppo di un'interfaccia per scegliere le notifiche da ricevere | 6/8/12 | **8 h** | **3 gg** | Alex | Dip. da WBS.6.1.2 |
| WBS.6.1.4 | Trigger automatici | 2/3/4 | **3 h** | **1 gg** | Alice | Dip. da WBS.6.1.1 |
| **Totale RBS.6** | | | **40 h** | **14 gg** | | Alice: **32 h (11 gg)**, Alex: **8 h (3 gg)** |
| **RBS.7 — Requisiti Non Funzionali** | | | | | |Tutti i punti sotto richiedono la terminazione di tutti i task di R1 |
| WBS.7.1.1 | Performance test | 8/12/16 | **12 h** | **4 gg** | Alice | — |
| WBS.7.2.1 | Monitoraggio crash | 8/12/16 | **12 h** | **4 gg** | Alice | — |
| WBS.7.3.1 | Valutazione GDPR e consensi | 8/12/16 | **12 h** | **4 gg** | Alex | — |
| WBS.7.4.1 | Conformità store | 8/12/16 | **12 h** | **4 gg** | Alex | — |
| WBS.7.5.1 | Rispetto accessibilità base | 8/12/16 | **12 h** | **4 gg** | Alex | — |
| **Totale RBS.7** | | | **60 h** | **20 gg** | | Alice: **24 h (8 gg)**, Alex: **36 h (12 gg)** |
| **TOTALE COMPLESSIVO PROGETTO** | | | **573 h** | **201 gg** | | Alice: 297h (104gg), Alex: 276h (97gg)|

---

## Fabbisogno Complessivo (Sintesi)

Si prevede che, considerando che sia Alice che Alex lavorino nei giorni infra-settimanali, lo sviluppo dell'applicazione richiede circa 21 settimane, ovvero 5 mesi. Si considera questa una stima approssimativa: non sono tenuti conto dei vincoli tra i vari requisiti (che possono ritardare le partenze di alcuni task) e di periodi di vacanze (natale/pasqua) che vanno a diminuire i giorni lavorativi. Nel Gannt, si otterranno delle stime più realistiche.

| Ruolo | FTE / mesi | Periodo | Vincoli / Note |
|--------|-------------|----------|----------------|
| PM/Dev — Alex | 0,5 | M1–M3 | Sessioni universitarie, priorità backend |
| Dev/UX — Alice | 0,5 | M1–M3 | UI e frontend |
| Totale stimato | ≈743 h | ≈3 mesi | 15 h/sett per persona (3 h/giorno effettive) |

---

