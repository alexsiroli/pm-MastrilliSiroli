# 2203 — Work Breakdown Structure (WBS) — Ziradò

Scopo: dettagliare il lavoro necessario per i deliverable della RBS, fino a task stimabili.

## Convenzioni
- Codifica: WBS.X.Y.Z (pacchetto → sotto‑pacchetto → attività)

## Struttura
```
WBS.1 Project Management
  WBS.1.1 Pianificazione e JPPS
  WBS.1.2 Monitoraggio e report
  WBS.1.3 Chiusura
WBS.2 UX/UI
  WBS.2.1 Wireframe mappa/eventi
  WBS.2.2 UI componenti principali
  WBS.2.3 Store listing (screenshot, descrizioni)
WBS.3 Backend/API
  WBS.3.1 Setup progetto e DB
  WBS.3.2 Servizi Luoghi
  WBS.3.3 Servizi Eventi
  WBS.3.4 Autenticazione minima/Admin
WBS.4 Mobile App
  WBS.4.1 Shell app, navigazione
  WBS.4.2 Vista mappa e marker
  WBS.4.3 Lista/filtri eventi
  WBS.4.4 Dettaglio evento/luogo
  WBS.4.5 Analytics base
WBS.5 Admin Portal
  WBS.5.1 CRUD luoghi
  WBS.5.2 CRUD eventi
WBS.6 Content Onboarding
  WBS.6.1 Raccolta dati luoghi
  WBS.6.2 Calendario eventi iniziale
WBS.7 QA & Release
  WBS.7.1 Test plan e smoke test
  WBS.7.2 Beta TestFlight/Closed Track
  WBS.7.3 Submission store
WBS.8 Growth/Marketing
  WBS.8.1 Landing e materiali promo
  WBS.8.2 Outreach esercenti
```

## Dizionario WBS (Estratto)
| ID | Nome | Descrizione | Output | Criteri di Completamento | Dipendenze | Effort (O/M/P) | Durata (O/M/P) | Owner |
|---|---|---|---|---|---|---|---|---|
| WBS.3.2 | Servizi Luoghi | API CRUD luoghi | Endpoint v1 | Test unit + doc | WBS.3.1 | 10/12/16h | 2/3/4g | Alex |
| WBS.4.2 | Vista mappa | UI mappa + marker | Vista funzionante | P95<2s, 3 device | WBS.3.2 | 12/16/20h | 3/4/5g | Alice |
| WBS.7.3 | Submission store | Requisiti store | App inviata | Checklist store ok | WBS.7.2 | 6/8/12h | 2/3/4g | Alex |

### Policy livello di dettaglio
Si scompone fino a task stimabili entro 2–5 giorni di lavoro, con chiari criteri di completamento. Task più grandi sono “epic” e vengono ulteriormente raffinati in fase di planning dello sprint.
