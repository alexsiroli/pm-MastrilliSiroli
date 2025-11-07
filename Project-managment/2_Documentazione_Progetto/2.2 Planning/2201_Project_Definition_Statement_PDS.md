# 2201 — Project Definition Statement (PDS) — Ziradò

Scopo: base di riferimento pre‑esecutiva per R1, con deliverable, piano, risorse, rischi e metriche in linea con POS, RBS e WBS.

## Metadati
- Progetto: Ziradò — Versione/Data: v1.1 / 2025‑11‑07 — Autori: Alex Siroli, Alice Mastrilli — Approvazioni: Docente

## 1) Visione e Obiettivi
- Visione: app unica per scoprire e vivere Cesena, aumentando l’engagement di residenti e turisti e la visibilità/ricavi dei locali.
- Release e ambito: R1 — mappa + eventi; R2 — coupon; R3 — recensioni con moderazione.
- Target temporali: R1 pubblicata sugli store entro 31/07/2026; R2 entro 6 mesi da R1; R3 entro 6 mesi da R2.

## 2) Deliverable e Requisiti
- Deliverable principali: App mobile (iOS/Android), Backend/API, Portale Admin, Sistema Notifiche, Contenuti iniziali, Documentazione.
- Ambito funzionale (RBS):
  - RBS.1 Mappa (schede locali, geolocalizzazione, filtri/tipologie)
  - RBS.2 Eventi (dettaglio, caricamento da gestori, calendario/lista con filtri)
  - RBS.3 Coupon/Offerte (R2)
  - RBS.4 Recensioni con moderazione (R3)
  - RBS.5 Backend/API e Admin (autenticazione/ruoli, operazioni ordinarie)
  - RBS.6 Sistema di Notifiche
  - RBS.7 Requisiti non funzionali (performance, stabilità, privacy, store, accessibilità)

### 2.1 Criteri di accettazione di alto livello
- Performance/stabilità: P95 < 2s sulle viste principali; crash/sessione < 1%.
- Store compliance: superamento validazioni automatiche e requisiti 100% soddisfatti (iOS/Android).
- Dati/geo: copertura iniziale ≥ 75% dei locali d’interesse; accuratezza media geolocalizzazione < 50m.
- Eventi/coupon: pubblicazione entro 5 minuti dalla creazione da parte dei gestori; limiti di utilizzo rispettati.
- Notifiche: ricezione confermata su iOS e Android (≥ 5 device test) e preferenze utente selezionabili.
- Privacy/GDPR: consensi espliciti raccolti; policy trasparenti; minimizzazione dati.
- Accessibilità: rispetto WCAG 2.1 AA sulle viste principali.

## 3) WBS (Sintesi) e Dizionario
- Struttura WBS: vedi 2202 (organizzazione per RBS → WBS.n.m).
- Macro‑pacchetti: 1 PM, 2 UX/UI, 3 Backend/API, 4 Mobile App, 5 Admin, 6 Content Onboarding, 7 QA, 8 Release/Store, 9 Marketing.
- Dizionario: per ciascun task DoR/DoD, owner e dipendenze (rif. 2202).

## 4) Pianificazione
- Milestone R1: JPPS; Freeze scope R1; Beta interna; Submission store; Go‑Live entro 31/07/2026.
- Milestone R2/R3: pianificazione e rilascio entro +6 mesi ciascuna da release precedente.
- Critical Path R1: Backend → Mobile → Integrazione → QA → Store (rif. 2203).

### 4.1 Dipendenze esterne
Policy store, limiti free tier mappe, disponibilità/risposta esercenti e referenti locali, accesso a dati/asset. Alternative: ottimizzazione asset, caching client, stage‑rollout, spostamento feature non critiche.

## 5) Risorse
- Team: 2 persone, capacità media 20h/sett ciascuno. Competenze: mobile/UX; backend/infra. Supporto tester ad hoc.

## 6) Costi e Budget
- Costi vivi: ~35–50€ setup + 10€/mese hosting; mappe in free tier; extra 0–50€.
- Valorizzazione ore interne (fuori bilancio corso): ~300h → 7.500€ (25€/h). Riserva gestionale: 10%.

## 7) Rischi e Mitigazioni
- Adozione bassa / concorrenza social → partnership con locali/Comune, piano contenuti, campagne mirate.
- Review store ritardata → buffer 2 settimane, beta test anticipato, check pre‑submission.
- Contenuti scarsi / poco attrattivi → outreach esercenti, linee guida contenuti, automazione ingest.
- Compliance GDPR → privacy policy, minimizzazione dati, revisione consensi.

## 8) Governance e Comunicazione
- Stand‑up settimanale; review quindicinale; status bisettimanale a sponsor; decision log nel repo.

## 9) Metriche di Successo
- Adozione: ≥ 5.000 download cumulati e rating medio ≥ 4.0/5 nei primi 12 mesi.
- Engagement esercenti: 75% dei locali del centro storico presenti entro 12 mesi; ≥ 20% dei locali pubblica eventi/coupon con cadenza mensile.
- Qualità tecnica: P95 < 2s; crash/sessione < 1%.
- Retention: ≥ 25% utenti attivi a D30.
- Ricavi: ≥ €10.000 nel primo anno; break‑even entro 12 mesi dal rilascio.

## 10) Baseline e Change Control
- Baseline scope/tempo/costi approvate; SCR (2303) per modifiche; aggiornamento Gantt/budget post approvazione.

## 11) Approvazioni
| Ruolo | Nome | Firma | Data |
|---|---|---|---|
| Sponsor | Docente | — | 2025‑11‑07 |
| PM | Alex Siroli | — | 2025‑11‑07 |
| PM | Alice Mastrilli | — | 2025‑11‑07 |
