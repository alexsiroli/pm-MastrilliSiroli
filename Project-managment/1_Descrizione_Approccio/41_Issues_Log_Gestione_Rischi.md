# 41 — Issues Log e Gestione dei Rischi: Procedura (Ziradò)

Scopo: definire processo e strategia di escalation per issues e rischi, con KPI e ruoli per il progetto.

## 1) Processo Issues
1. Identificazione e registrazione (2403)
2. Triage P1/P2/P3 e prioritizzazione (impatto×urgenza)
3. Assegnazione (owner, SLA) e piano d’azione
4. Risoluzione, verifica e test regressione
5. Chiusura e lesson learned

## 2) Problem Escalation Strategy
- Livelli: Team → PM owner area → Sponsor/Docente (se milestone a rischio)
- SLA: P1 48h, P2 5gg, P3 backlog; canali: tracker + ping diretto
- Criteri: impatto su CP, utenti, compliance, reputazione

## 3) Rischi Residui
- Monitorare trigger (es. ritardi store, picchi API mappe)
- Attivare contingenze (es. ridurre scope, disattivare feature opzionali)

## 4) Struttura Issues Log (vedi 2403)
- Campi minimi: ID, data, descrizione, impatto, owner, priorità, stato, azioni, data chiusura

## 5) Ruoli e Responsabilità (RASCI sintetica)
- R: Owner issue/rischio
- A: PM del dominio (Alex backend/infra; Alice mobile/UX)
- S: Tester/SME
- C: Stakeholder (docente, referenti locali)
- I: Team allargato

## 6) KPI e Monitoraggio
- MTTR (tempo medio risoluzione), aging issues, % P1 rispettate, difetti per release

### 6.1 Esempi pratici
Se una P1 (crash critico) non è risolta entro 48h, si attiva escalation al docente con proposta di piano (hotfix, rollback, disattivazione temporanea feature) e comunicazione sintetica dell’impatto.

## 7) Template Voce Issues (Esempio)
| Campo | Valore |
|---|---|
| ID | ISS‑001 |
| Data | 2025‑02‑20 |
| Descrizione | Crash su vista dettagli evento su Android 14 |
| Impatto | Alto |
| Priorità | P1 |
| Owner | Alice |
| Azioni | Riprodurre, fixare, release hotfix beta |
| Stato | In corso |
| Data Chiusura | — |
