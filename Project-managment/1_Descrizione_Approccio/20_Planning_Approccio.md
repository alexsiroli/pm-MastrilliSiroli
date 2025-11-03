# 20 — Planning: Approccio (CesenaLive)

Scopo: definire WBS, stime, sequenza e schedula per l’MVP (R1) e la roadmap (R2‑R3), con baseline di scope/tempo/costi.

## 1) Dalla RBS alla WBS
- Criteri: deliverable‑based per feature (Mappa, Eventi, Coupon, Recensioni) e abilitatori (Backend, Admin, Content, QA, PM).
- Convenzioni ID: RBS.X.Y ↔ WBS.X.Y.Z; dizionario WBS con DoR/DoD per ogni task.

## 2) Metodi di Stima
- Three‑Point (O/M/P) su effort/durata; consenso tra Alex e Alice.
- Riferimenti: storici personali e benchmark di librerie/scaffold.

### 2.1 Dettaglio calcolo e incertezza
Per ogni attività si stimano tre valori: Ottimistico (O), Probabile (M), Pessimistico (P). La stima attesa è E = (O + 4M + P) / 6; la varianza è σ² = ((P − O) / 6)². Le attività sul cammino critico ricevono buffer mirati (risk‑based), mentre le non critiche tollerano ritardi entro il float.

## 3) Sequenziamento e Dipendenze
- FS prevalenti; lead per UI/Copy in parallelo; integrazione mappe prima dei filtri eventi; backend pronto prima dell’app.
- Network Diagram centrato su: Design → Backend → Mobile → Integrazione → QA → Store.

## 4) Schedula e Critical Path
- R1 (MVP) 10–12 settimane: CP atteso su Backend API → Mobile Eventi → Integrazione → QA → Approvazione Store.
- Slack su Content Onboarding e Marketing iniziale.

### 4.1 Analisi del rischio di schedula
Il rischio principale è la revisione store: anche a parità di qualità, i tempi possono variare. Viene perciò previsto un buffer di 1–2 settimane tra RC e Go‑Live. Un secondo rischio è la qualità/quantità contenuti: mitigato avviando l’onboarding in parallelo allo sviluppo.

## 5) Risorse e Livellamento
- Alex: 50–60% su backend/infra/PM; Alice: 50–60% su mobile/UX/content. Supporto test esterno (amici/studenti).
- Livellamento: limitare WIP a 2 task/persona; sprint bisettimanali.

## 6) Baseline
- Scope baseline: R1 feature minime; R2 coupon; R3 recensioni.
- Tempo/Costo baseline: Gantt e budget in 2204/2206; change control via SCR (2303).

## 7) Governance e Comunicazione
- Stand‑up settimanale, review ogni 2 settimane, retro al termine di ogni release.
- Canali: repo + issue tracker; doc in Drive/Notion; stakeholder update quindicinale.

## 8) Misurazione dell’Avanzamento
- Burn‑down per sprint; milestone chart; EVA semplice (SPI/CPI) su R1.

### 8.1 Criteri di ricalibrazione
Se SPI o CPI < 0,9 per due periodi consecutivi, si applica una ricalibrazione del backlog (riduzione scope non critico, concentrazione su bug/CP, incremento pairing).

## 9) Checklist
- [x] RBS completa e tracciata
- [x] WBS con dizionario attività
- [x] Stime validate e fonti
- [x] Schedula con cammino critico
- [x] Baseline approvate (scope, tempo, costi)
