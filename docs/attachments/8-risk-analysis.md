---
layout: page
title: 8-risk-analysis.md – Analisi Rischi e Mitigazione
permalink: /attachments/8-risk-analysis/
---

# **Analisi Rischi e Mitigazione — Ziradò**

## **1) Metodo e scala di valutazione**

* **Probabilità (P):** 1 molto bassa · 5 molto alta
* **Impatto (I):** 1 trascurabile · 5 critico (ritardi > 4 settimane / danno reputazionale / rischio legale)
* **Priorità (Score):** **R = P × I** ⇒ **Basso** (1–6) · **Medio** (7–12) · **Alto** (13–25)
* **Strategie:** **Evitare / Mitigare**
* **Owner rischio:** ruolo primario responsabile del monitoraggio e delle azioni

---

## **3) Registro dei rischi**

| **ID** | **Descrizione**                 | **Causa**                 | **Conseguenza**    | **P** | **I** | **R** | **Owner** | **Strategia** | **Azioni di mitigazione**                                            | **Trigger/Indicatori**      | **Contingenza (fallback)**                            |
| ------ | ------------------------------- | ------------------------- | ------------------ | ----: | ----: | ----: | --------- | ------------- | -------------------------------------------------------------------------- | --------------------------- | ----------------------------------------------------- |
| R-01   | Rejection/ritardi store         | Linee guida non allineate | Ritardo nella pubblicazione       |     3 |     5 |    15 | Alex      | Mitigare      | Assicurarsi che **RBS.8.4** sia completato correttamente                | 1° rifiuto o tempi di review superiori ai 5 giorni   | Ridurre scope release           |
| R-02   | Basso engagement esercenti      | Valore percepito basso    | Pochi contenuti    |     4 |     4 |    16 | Alex      | Mitigare      | Contatto diretto con almeno 20 locali, fornire template eventi | <15 locali attivi in 4 sett | Incentivi per i primi locali |
| R-03   | Sforamento tempi (team ridotto) | Impegni universitari, imprevisti         | Ritardi a cascata |     4 |     4 |    16 | Alice     | Mitigare      | Inserire un buffer del 10% sui tempi di completamento               | <80% task completi in tempo        | Spostamento di alcune funzioni a R2/R3                |
| R-04   | Dati incompleti/errati          | Modifiche non notificate          | Esperienza utente negativa        |     3 |     4 |    12 | Alex      | Mitigare      | Controllo manuale periodico                    | Segnalazioni di incoerenza sul 2% dei dati            | Richiesta di inserimento da parte degli utenti segnalatori                              |
| R-05   | Performance lente/crash         | Gestione UI non ottimale     | Esperienza utente negativa       |     3 |     4 |    12 | Alice     | Mitigare      |Assicurarsi che **RBS.8.1/RBS.8.2** siano completati                                | p95>2s o crash>1%           | Rollback a versione precedente                          |
| R-06   | GDPR/consensi carenti           | Policy incomplete  | Rischio legale     |     2 |     5 |    10 | Alex      | Evitare       | Assicurarsi che **RBS.8.3** sia completato correttamente                             | Controllo interno fallito       | Disabilitare le funzioni a rischio                       |
| R-07   | Abusi recensioni                | Spam/troll                | Danno reputazione  |     2 |     5 |    10 | Alice     | Mitigare      | Impostare un rate limit, limitare gli utenti più segnalati     |  più di 5 segnalazioni al giorno           | Moderazione manuale accelerata                        |
| R-08   | Ricavi < target                 | Sponsor insufficienti             | No break-even      |     3 |     4 |    12 | Alex      | Mitigare      | Assicurarsi che **RBS.8.3** sia completato correttamente e ricerca attiva di sponsor                                          | Break Even Point non raggiunto in 6 mesi              | Sconti per locali
| R-09   | UX non chiara                   | Navigazione complessa     | Abbandono da parte degli utenti          |     3 |     3 |     9 | Alex      | Mitigare      | Beta test con almeno 20 utenti                                                  | Meno del 25% degli utenti continua a utilizzare l’app 30 giorni dopo il primo accesso          | Semplificare la UI per favorire semplicità                                   |
