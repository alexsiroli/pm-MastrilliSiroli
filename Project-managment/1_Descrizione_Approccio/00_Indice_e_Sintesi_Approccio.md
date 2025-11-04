# 00 — Indice e Sintesi dell'Approccio (Ziradò)

Scopo: introdurre l’approccio di Project Management scelto per “Ziradò”, app mobile che centralizza eventi, attività e locali della città di Cesena per favorire turismo locale e coinvolgimento dei cittadini.

## 1) Modello PMLC scelto
- Modello: Ibrido Iterativo‑Incrementale, con timebox a sprint e milestone fisse (pilot locale → estendibile).
- Ragioni della scelta: requisiti core noti ma forte incertezza su adozione, contenuti e UX; team ridotto (2 persone); necessità di rilasci progressivi per testare valore e raccogliere feedback.
- Implicazioni operative: pianificazione iniziale del MVP e milestone, backlog dinamico, change control leggero, misurazione continua dei KPI d’adozione.

## 2) Contesto e Assunzioni
- Target: cittadini e turisti di Cesena; esercenti e associazioni locali.
- Vincoli: ambito territoriale iniziale, tempo limitato dell’elaborato, budget minimo, policy store (Apple/Google), GDPR.
- Assunzioni: disponibilità di contenuti dai locali, sponsorship iniziale da entità locali, mappe con free tier sufficiente, hosting low‑cost.
- Tecnologie (ipotesi): mobile cross‑platform, backend REST, DB cloud, mappe (OpenStreetMap/Mapbox), analytics.

## 3) Indicatori di Successo e Metriche
- IRACIS: Increase Revenue (incremento spesa locale via coupon), Avoid Cost (riduzione dispersione info per i cittadini), Improve Service (unico punto di accesso eventi/attività/luoghi).
- KPI: MAU ≥ 500 (M2), ≥ 1.500 (M3); ≥ 50 eventi attivi/mese (M2); ≥ 30 esercenti registrati (M3); Retention D30 ≥ 20%; Rating store ≥ 4.0; Conversione coupon ≥ 5% utenti attivi; Sponsorship ≥ 2 entro M3.
- Soglie e early warning: SPI/CPI < 0,9 → azione correttiva; MAU < 60% target → sprint dedicato a growth/UX.

## 4) Indice dei Documenti (Approccio)
- 10_Scoping_Initiating_Approccio.md
- 11_Meeting_Scoping_Sintesi.md
- 20_Planning_Approccio.md
- 21_Meeting_Planning_JPPS_Sintesi.md
- 30_Launching_Execution_Approccio.md
- 31_Meeting_Kickoff_Sintesi.md
- 40_Monitoring_Controlling_Approccio.md
- 41_Issues_Log_Gestione_Rischi.md
- 50_Closing_Approccio.md

## 5) Indice dei Documenti (Documentazione di Progetto)
- POS, Stakeholder Analysis, PDS
- RBS, WBS, Schedula, Stime e Risorse, Budget, Cash Flow
- Analisi Rischi e Mitigazione, Project Proposal
- Team Operating Rules, RASCI, Scope Change Request
- Status Report, Impact Statement, Issues Log, EVA
- Accettazione Cliente, Audit Post‑Implementazione, Rapporto Finale

## 6) Sintesi dell’Approccio
- Strategia MVP in 3 release: R1 (MVP: mappa + eventi), R2 (coupon + schede locali), R3 (recensioni + growth features).
- Governance leggera: stand‑up settimanale, review sprint bisettimanale, demo a sponsor/committente (docente) a fine milestone.
- Rischi prioritari: bassa adozione, qualità/aggiornamento contenuti, compliance store e GDPR. Mitigazioni: partnership locali, automazione ingest contenuti, early test su TestFlight/Closed Track.

### 6.1 Razionale di scelta del modello (discorsivo)
L’incertezza principale non riguarda tanto il “cosa” consegnare nel MVP (mappa ed eventi sono chiari), quanto il livello di adozione e la qualità/aggiornamento dei contenuti nel tempo. Un modello ibrido iterativo‑incrementale consente di rilasciare valore presto (R1) e testare ipotesi chiave (es. quali categorie eventi interessano di più), mantenendo tuttavia milestone e baseline per dare disciplina al lavoro. In tal modo, il progetto rimane focalizzato su un set ridotto di funzionalità core, rimandando elementi più rischiosi o accessori (coupon, recensioni) a release successive. Questo riduce il rischio complessivo, migliora il time‑to‑learning e ottimizza l’uso di un team piccolo.

### 6.2 Piano di scala (dal pilota a estensioni)
Il perimetro cittadino di Cesena è un pilota gestibile per contenuti e partnership. Una volta validati i KPI di adozione e l’onboarding dei partner locali, sarà possibile replicare il modello su altre città, mantenendo la stessa architettura e processi (multi‑tenant o multi‑istanza) con adattamenti minimi a tassonomie locali.

## 7) Riferimenti
- PMBOK 7th, Agile (Scrum/Kanban), PRINCE2 (light), Lean UX.
- Tool ipotizzati: GitHub, CI/CD, tracker, Notion/Drive, Map SDK, Firebase/Analytics.

### 7.1 Collegamenti tra standard e pratiche adottate
L’impostazione segue i domini di performance del PMBOK (Stakeholder, Team, Development Approach & Life Cycle, Planning, Project Work, Delivery, Measurement, Uncertainty). Scrum/Kanban guidano la gestione del flusso (timebox, WIP, review), mentre PRINCE2 “light” informa la governance (baselines, change control, business case). Lean UX orienta a rilasci frequenti e apprendimento da dati.

## Checklist Rapida
- [x] Modello PMLC motivato
- [x] Assunzioni e vincoli chiave
- [x] Metriche e soglie definite
- [x] Indice documenti completo
