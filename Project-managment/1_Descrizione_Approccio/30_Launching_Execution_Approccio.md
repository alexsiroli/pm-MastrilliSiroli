# 30 — Launching/Execution: Approccio (Ziradò)

Scopo: avviare l’esecuzione R1 con organizzazione del team, regole operative, qualità e change control.

## 1) Organizzazione del Team
- Team: 2 studenti (Alex — backend/infra/PM; Alice — mobile/UX/content). Supporto: tester amici/studenti (ad hoc).
- Responsabilità: Alex (API, dati, CI/CD, store back‑office); Alice (UI mobile, mappe, eventi, contenuti, store listing).

## 2) Regole Operative
- Problem Solving: A3 + 5‑why; ticket con root cause; timebox 1 giorno per indagine.
- Decision Making: consenso; se bloccati → decide PM owner area; escalation a Sponsor se impatta milestone.
- Comunicazione: stand‑up settimanale (30’), sync rapido mid‑week; retro per release.
- DoR/DoD: requisito chiaro, mock, dati minimi; DoD con test, review, doc, analytics.

## 3) Gestione Cambiamenti di Scope
- Richieste tramite SCR (2303); valutazione impatti (tempo/costi/qualità/risorse) e priorità.
- Scope Bank: backlog “candidati” post‑MVP; si proteggono milestone R1.

## 4) Qualità, Tooling e Cadence
- QA: checklist smoke, test su 3 device, beta testing; bug triage P1‑P3.
- Tool: GitHub, CI/CD, tracker issue, Map SDK, Analytics, Crashlytics.
- Cadence: sprint 2 settimane, release candidate alla quarta settimana.

### 4.1 Readiness Operativa
Prima della RC, si esegue una “go/no‑go checklist” che include: copertura flussi critici, performance su rete 4G, accessibilità minima (contrasti, font), privacy policy integrata, materiali store (screenshot, descrizioni) pronti.

## 5) Fornitori e Terze Parti
- Map provider (free tier); store Apple/Google; email/analytics provider. Verifica T&C e limiti.

## 6) Knowledge Management
- Doc tecnica e decision log in repo/Drive; changelog rilasci; versioning semantico.

### 6.1 Pipelines contenuti
Per assicurare aggiornamento, si definisce un flusso: (1) ingest manuale iniziale dei luoghi/eventi da fonti locali; (2) submission semplificata per esercenti; (3) revisione minima; (4) pubblicazione. Metriche: tempo di pubblicazione medio, tasso di contenuti rifiutati.

## 7) Checklist
- [x] Team ingaggiato e informato
- [x] Regole operative pubblicate
- [x] Processo change approvato
- [x] Cadence e tool definiti
