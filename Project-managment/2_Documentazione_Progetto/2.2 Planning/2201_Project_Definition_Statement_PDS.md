# 2201 — Project Definition Statement (PDS) — CesenaLive

Scopo: base di riferimento pre‑esecutiva per R1, con deliverable, piano, risorse, rischi e metriche.

## Metadati
- Progetto: CesenaLive — Versione/Data: v1.0 / 2025‑02‑10 — Autori: Alex Siroli, Alice Mastrilli — Approvazioni: Docente

## 1) Visione e Obiettivi
- Visione: app unica per scoprire e vivere Cesena.
- Obiettivi R1: mappa+eventi; R2: coupon; R3: recensioni. KPI: MAU, rating, eventi attivi, esercenti onboarded, redemption coupon.

## 2) Deliverable e Requisiti
- Vedi RBS (2202). Deliverable principali: App mobile (iOS/Android), Backend/API, Admin portal, Contenuti iniziali, Documentazione.

### 2.1 Criteri di accettazione di alto livello
- App: performance P95 < 2s nelle viste principali; crash < 1%; navigazione coerente.
- Backend: endpoint core per luoghi/eventi con test di integrazione; logging e basic monitoring.
- Contenuti: seed iniziale curato con copertura minima per categorie principali.

## 3) WBS (Sintesi) e Dizionario
- WBS macro: 1 PM, 2 UX/UI, 3 Backend/API, 4 Mobile App, 5 Admin, 6 Content Onboarding, 7 QA, 8 Release/Store, 9 Marketing.
- Dizionario: per ciascun task DoR/DoD, owner, dipendenze (vedi 2203).

## 4) Pianificazione
- Milestone: JPPS, RC (sett. 8), Go‑Live (sett. 10–12). CP: Backend → Mobile → Integrazione → QA → Store (2204).

### 4.1 Dipendenze esterne
Policy store, limiti free tier mappe, disponibilità referenti locali. Prevedere alternative: riduzione immagini pesanti, caching lato client, spostamento di feature non critiche.

## 5) Risorse
- Team 2 persone, capacità media 20h/sett ciascuno. Competenze: mobile/UX, backend/infra. Supporto tester ad hoc.

## 6) Costi e Budget
- Vivi: ~35–50€ setup + 10€/mese hosting; mappe free tier; extra 0–50€.
- Valorizzazione ore interne (non a bilancio corso): ~300h → 7.500€ (25€/h). Riserve gestionali: 10%.

## 7) Rischi e Mitigazioni
- Adozione bassa → partnership locali, growth sprint.
- Review store ritardata → buffer 2 settimane, beta test anticipato.
- Contenuti scarsi → outreach esercenti, automazione ingest.
- Compliance GDPR → privacy policy, consulenza risorse online, minimizzazione dati.

## 8) Governance e Comunicazione
- Stand‑up settimanale, review ogni 2 settimane; status bisettimanale a sponsor; decision log in repo.

## 9) Metriche di Successo
- MAU, rating, eventi attivi, esercenti onboarded, retention D30, redemption coupon.

## 10) Baseline e Change Control
- Baseline scope/tempo/costi approvate; SCR (2303) per modifiche; update Gantt/budget post approvazione.

## 11) Approvazioni
| Ruolo | Nome | Firma | Data |
|---|---|---|---|
| Sponsor | Docente | — | 2025‑02‑10 |
| PM | Alex Siroli | — | 2025‑02‑10 |
| PM | Alice Mastrilli | — | 2025‑02‑10 |
