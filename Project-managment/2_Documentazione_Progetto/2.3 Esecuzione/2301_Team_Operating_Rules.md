# 2301 — Team Operating Rules — Ziradò

Scopo: regole operative del team (2 persone) per R1–R3.

## Comunicazioni
- Canali: tracker issue + chat; meeting settimanale (30’); retro a fine release.
- Tempi risposta: entro 24h nei giorni lavorativi.

## Decision Making
- Consenso informato; in caso di stallo decide l’owner dell’area (Alex backend/infra, Alice mobile/UX).

## Problem Solving
- A3 + 5‑why; ticket con causa radice, azioni e validazione fix.

## Gestione Conflitti
- Confronto diretto; se persiste, timebox 24h e decisione PM owner; escalation al docente se impatta milestone.

## Tool e Pratiche
- Git branching feature‑branch; PR con review reciproca; CI su main; tag release.

### Linee guida di qualità del codice
- Stile coerente con formatter del linguaggio; commit piccoli e descrittivi; PR con descrizione di scopo, screen/recording quando UI.
- Test minimi sui servizi core; feature flag per funzionalità non finali.

## Definition of Ready / Done
- DoR: user story chiara, mockUI, dati, criteri accettazione.
- DoD: codice testato, review 1+, analytics/tracking, doc aggiornata.

## SLA Interni
- PR review: <48h; bug P1: <48h; P2: <5gg.

### Incident management
In caso di regressioni critiche in beta, apertura immediata di un incident con comunicazione al docente e piano d’azione (rollback/hotfix), poi post‑mortem breve con lesson learned.

## Checklist Rapida
- [x] Canali e cadenze stabiliti
- [x] DoR/DoD pubblicate
- [x] SLA condivisi
