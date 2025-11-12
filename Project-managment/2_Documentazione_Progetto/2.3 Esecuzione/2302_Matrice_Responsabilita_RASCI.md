# 2302 — Matrice di Responsabilità RASCI — Ziradò
DISCUTERE: SERVE VERAMENTE? 

Scopo: mappare deliverable principali con i ruoli del team e stakeholder.

## Ruoli
- PM (Alex)
- Backend (Alice)
- Frontend e UX (Alex)
- QA/Test – test funzionali/regressione/usabilità
- Build & Store (pubblicazione) (Alex o Alice)
- Legal/Compliance – privacy/GDPR, policy (Alex o Alice)
- Stakeholder (Clienti/Esercenti/Comune)
---

### RBS.1 — Mappa

| **WBS**                                  | **PM** | **Backend** | **Frontend** | **QA** | **Build&Store** | **Legal** | **Stakeholder** |
| ---------------------------------------- | ------ | ----------- | ------------ | ------ | --------------- | --------- | --------------- |
| **1.1.1** Modello dati scheda locale     | **A**  | **R**       |    **S**          | **C**  |            |           | **I**           |
| **1.1.2** Raccolta info locali           | **A**  |     **I**   |     **R**         | **C**  |            |           | **S**           |
| **1.1.3** CRUD locali + permessi         | **A**  | **R**       |              | **C**  | **S**           |           | **I**           |
| **1.1.4** Azioni rapide (call/map/share) | **A**  |             | **R**        | **C**  | **S**           |           | **I**           |
| **1.2.1** Mappa UI/gesture               | **A**  |             | **R**        | **C**  | **S**           |           | **I**           |
| **1.2.2** Geocoding indirizzi            | **A**  | **R**       |              | **C**  | **S**           |           | **I**           |
| **1.2.3** Load punti su mappa            | **A**  | **R**       |              | **C**  | **S**           |           | **I**           |
| **1.3.1** Tipologie locali               | **A**  | **R**       |              | **C**  | **S**           |           | **I**           |
| **1.3.2** Filtri tipologia/orari/prezzo  | **A**  |             | **R**        | **C**  | **S**           |           | **I**           |

---

### RBS.2 — Eventi

| **WBS**                         | **PM** | **Backend** | **Frontend** | **QA** | **Build&Store** | **Legal** | **Stakeholder** |
| ------------------------------- | ------ | ----------- | ------------ | ------ | --------------- | --------- | --------------- |
| **2.1.1** Modello dati evento   | **A**  | **R**       |              | **C**  | **S**           |           | **I**           |
| **2.2.1** CRUD eventi (gestori) | **A**  | **R**       |              | **C**  | **I**           |           | **S**           |
| **2.2.2** Validazioni form      | **A**  |             | **R**        | **C**  | **I**           |           | **S**           |
| **2.3.1** Calendario (UI)       | **A**  |             | **R**        | **C**  | **S**           |           | **I**           |
| **2.3.2** Lista eventi (UI)     | **A**  |             | **R**        | **C**  | **S**           |           | **I**           |
| **2.3.3** Filtri eventi         | **A**  |             | **R**        | **C**  | **S**           |           | **I**           |

---

### RBS.3 — Coupon/Offerte (R2)

| **WBS**                            | **PM** | **Backend** | **Frontend** | **QA** | **Build&Store** | **Legal** | **Stakeholder** |
| ---------------------------------- | ------ | ----------- | ------------ | ------ | --------------- | --------- | --------------- |
| **3.1.1** Modello dati coupon      | **A**  | **R**       |              | **C**  | **S**           |           | **I**           |
| **3.1.2** CRUD coupon (gestori)    | **A**  | **R**       |              | **C**  | **I**           |           | **S**           |
| **3.2.1** UI lista coupon (client) | **A**  |             | **R**        | **C**  | **S**           |           | **I**           |
| **3.2.2** Redeem in presenza       | **A**  |             | **R**        | **C**  | **I**           |           | **S**           |

---

### RBS.4 — Recensioni (R3)

| **WBS**                                         | **PM** | **Backend** | **Frontend** | **QA** | **Build&Store** | **Legal** | **Stakeholder** |
| ----------------------------------------------- | ------ | ----------- | ------------ | ------ | --------------- | --------- | --------------- |
| **4.1.1** Punti da valutare per tipologia       | **A**  | **R**       |              | **C**  | **S**           |           | **I**           |
| **4.1.2** Feature valutazione clienti           | **A**  |             | **R**        | **C**  | **S**           |           | **I**           |
| **4.1.3** Analisi punteggi                      | **A**  | **R**       |              | **C**  | **S**           |           | **I**           |
| **4.1.4** UI visualizzazione punteggi           | **A**  |             | **R**        | **C**  | **S**           |           | **I**           |
| **4.2.1** Modello recensione testuale           | **A**  | **R**       |              | **C**  | **S**           |           | **I**           |
| **4.2.2** UI scrittura recensione + validazioni | **A**  |             | **R**        | **C**  | **S**           |           | **I**           |
| **4.2.3** UI lista recensioni                   | **A**  |             | **R**        | **C**  | **S**           |           | **I**           |
| **4.3.1** Segnalazione/gestione inappropriati   | **A**  | **R**       |              | **C**  | **I**           |           | **S**           |
| **4.3.2** UI segnalazioni (clienti/gestori)     | **A**  |             | **R**        | **C**  | **S**           |           | **I**           |
| **4.3.3** UI moderazione admin                  | **A**  |             | **R**        | **C**  | **S**           |           | **I**           |

---

### RBS.5 — Backend/API e Admin

| **WBS**                                    | **PM** | **Backend** | **Frontend** | **QA** | **Build&Store** | **Legal** | **Stakeholder** |
| ------------------------------------------ | ------ | ----------- | ------------ | ------ | --------------- | --------- | --------------- |
| **5.1.1** Auth (email/Google)              | **A**  | **R**       | **S**        | **C**  |                 |           | **I**           |
| **5.1.2** UI coerente al ruolo             | **A**  | **S**       | **R**        | **C**  |                 |           | **I**           |
| **5.2.1** Portale Admin (CRUD/moderazione) | **A**  | **S**       | **R**        | **C**  |                 |           | **I**           |

---

### RBS.6 — Sistema di Notifiche

| **WBS**                                   | **PM** | **Backend** | **Frontend** | **QA** | **Build&Store** | **Legal** | **Stakeholder** |
| ----------------------------------------- | ------ | ----------- | ------------ | ------ | --------------- | --------- | --------------- |
| **6.1.1** Motore notifiche                | **A**  | **R**       |              | **C**  | **S**           |           | **I**           |
| **6.1.2** Trigger locali/eventi (clienti) | **A**  | **R**       |              | **C**  | **S**           |           | **I**           |
| **6.1.3** Preferenze utenti               | **A**  |             | **R**        | **C**  | **S**           |           | **I**           |
| **6.1.4** Trigger esiti per gestori       | **A**  | **R**       |              | **C**  | **S**           |           | **I**           |
| **6.2.1** Notifiche coupon (R2)           | **A**  | **R**       |              | **C**  | **S**           |           | **I**           |
| **6.2.2** Preferenze notif. coupon (R2)   | **A**  |             | **R**        | **C**  | **S**           |           | **I**           |
| **6.3.1** Notifiche moderazione (R3)      | **A**  | **R**       |              | **C**  | **S**           |           | **I**           |

---

### RBS.7 — Lancio & Sponsorizzazione

| **WBS**                                           | **PM** | **Backend** | **Frontend** | **QA** | **Build&Store** | **Legal** | **Stakeholder** |
| ------------------------------------------------- | ------ | ----------- | ------------ | ------ | --------------- | --------- | --------------- |
| **7.1.1** Asset store (descr./screenshot/privacy) | **A**  | **S**       | **R**        | **C**  |                 |           | **I**           |
| **7.1.2** Pubblicazione sugli store               | **A**  | **S**       |              | **C**  | **R**           |           | **I**           |
| **7.2.1** Pagina sponsor (UI)                     | **A**  | **S**       | **R**        | **C**  |                 |           | **I**           |
| **7.2.2** Slot advertising & placement            | **A**  | **S**       | **R**        | **C**  |                 |           | **I**           |
| **7.3.1** Setup canali social & brand             | **A**  | **S**       | **R**        | **C**  |                 |           | **I**           |
| **7.3.2** Piano editoriale & materiali            | **A**  | **S**       | **R**        | **C**  |                 |           | **I**           |
| **7.3.3** Scheduling/pubblicazione/community      | **A**  |             | **S**        | **C**  | **I**           |           | **R**           |
| **7.4.1** Submission aggiornamenti (R2/R3)        | **A**  | **S**       |              | **C**  | **R**           |           | **I**           |
| **7.4.2** Release notes & micro-campagna          | **A**  |             | **S**        | **C**  | **I**           |           | **R**           |

---

### RBS.8 — Requisiti Non Funzionali

| **WBS**                                  | **PM** | **Backend** | **Frontend** | **QA** | **Build&Store** | **Legal** | **Stakeholder** |
| ---------------------------------------- | ------ | ----------- | ------------ | ------ | --------------- | --------- | --------------- |
| **8.1.1** Performance (≤2s nel 95%)      | **A**  | **R**       |              | **C**  | **S**           |           | **I**           |
| **8.2.1** Stabilità (crash <1%)          | **A**  | **R**       |              | **C**  | **S**           |           | **I**           |
| **8.3.1** Privacy/GDPR (consensi/policy) | **A**  | **S**       |              | **I**  |                 | **R**     | **C**           |
| **8.4.1** Normative store                | **A**  | **S**       |              | **C**  | **I**           | **R**     |                 |
| **8.6.1** Re-test post-release           | **A**  | **C**       |              | **R**  | **S**           |           | **I**           |
| **8.6.2** Verifica privacy nuove build   | **A**  | **S**       |              | **C**  | **I**           | **R**     |                 |

---

Vuoi che te la prepari anche in **.md “pulito”** da incollare o in **.pptx** già impaginata con titolo e nota “Alex ricopre PM e (talvolta) Frontend”?
