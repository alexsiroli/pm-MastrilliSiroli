# 2203 — Schedula Gantt e Network Diagram — Ziradò

Documento basato su POS (2101), WBS (2202), stime risorse (2204) e budget (2205). Descrive la sequenza temporale delle release R1‑R3 e le dipendenze chiave per il network diagram.

## Assunzioni di schedulazione
- Capacità disponibile: 30 h/sett (15 h per persona) come da 2204; sprint bisettimanali.
- Baseline calendario: partenza **lunedì 01/12/2025**; settimane 24/12/2025–07/01/2026 e 01/04/2026–08/04/2026 sono non lavorative e vengono escluse dal conteggio.
- Unità temporale: **giorni effettivi** (3 h lavorative reali) convertiti in settimane di calendario.
- Vincoli POS: R1 (MVP) entro 31/07/2026; R2 e R3 entro 3 mesi uno dall’altro.
- Strategia: sviluppo incrementale → R1 (core), R2 (coupon), R3 (recensioni); ogni release include regressione non funzionale e submission store (WBS.7.4).
- Dipendenze: prevalentemente Finish‑to‑Start; alcune attività di content/marketing possono essere in Start‑to‑Start con i test finali.

## Roadmap 2025–2026
| Milestone/Release | Periodo | Durata stimata | Deliverable principali | Note |
|---|---|---|---|---|
| Kick-off + setup stack (M0) | 01/12/2025 – 14/12/2025 | 2 sett | Ambienti, login/admin base (WBS.5.1) | baseline processi PMLC ibrido |
| **R1 — Core (Mappa + Eventi + Notifiche)** | 15/12/2025 – 30/06/2026 | 20 sett + 3 sett buffer (al netto delle pause) | RBS.1, RBS.2, RBS.5, RBS.6, RBS.7, RBS.8 | Include stop 24/12–07/01 e 01/04–08/04; Go-Live previsto 03/07 |
| **R2 — Coupon & promo** | 08/07/2026 – 04/08/2026 | 4 sett | RBS.3, notifiche coupon, campagna update | Release 2 sugli store 08/08 |
| **R3 — Recensioni & moderazione** | 05/08/2026 – 15/09/2026 | 6 sett | RBS.4, notifiche recensioni, regressione | Release 3 e comunicazione finale 18/09 |
| Operatività e monitoraggio | Settembre–Dicembre 2026 | — | KPI, sponsorship, gestione contenuti | copre break-even entro 6 mesi dal lancio (POS) |

## Gantt R1 — macro-fasi e sprint
La schedula di R1 è articolata in 10 sprint bisettimanali (20 settimane). Ogni fase sotto aggrega i pacchetti WBS indicati in 2202/2204; la colonna “Timeline” mostra la posizione relativa sul semestre (▉ = una settimana).

| # | Fase (Sprint) | Periodo | Durata eff. (gg) | Timeline | WBS principali / Owner | Dipendenze & Output |
|---|---|---|---|---|---|---|
| 1 | Setup stack & governance | 01/12/2025 – 12/12/2025 | 9 | `▉▉` | WBS.5.1.1 (Alice), WBS.5.1.2 (Alex) | Kick-off → ambienti, autenticazione base, baseline backlog |
| 2 | Modello + dataset locali | 15/12/2025 – 17/01/2026 | 10 | `▉▉` | WBS.1.1.1 (Alice), WBS.1.1.2 (Alex) | FS da fase 1 → schema dati, raccolta info esercenti (pausa 24/12–07/01) |
| 3 | CRUD locali e azioni rapide | 20/01/2026 – 31/01/2026 | 12 | `▉▉▉` | WBS.1.1.3 (Alice), WBS.1.1.4 (Alex) | Richiede dataset stabile → gestione contenuti + quick actions |
| 4 | Geolocalizzazione & rendering mappa | 03/02/2026 – 07/03/2026 | 23 | `▉▉▉▉▉` | WBS.1.2.1/1.2.3 (Alice), WBS.1.2.2/1.2.4 (Alex) | Dipende da CRUD completato → mappa interattiva con punti accessibili |
| 5 | Tipologie e filtri | 09/03/2026 – 20/03/2026 | 10 | `▉▉` | WBS.1.3.1 (Alice), WBS.1.3.2 (Alex) | FS da geolocalizzazione → filtri mappa funzionanti |
| 6 | Sezione Eventi (data + UI) | 23/03/2026 – 03/05/2026 | 32 | `▉▉▉▉▉▉` | WBS.2.1–2.3 (Alice + Alex) | Richiede filtri attivi → calendario e lista eventi; pausa 01/04–08/04 |
| 7 | Portale admin e sponsor base | 09/04/2026 – 24/05/2026 | 13 | `▉▉▉` | WBS.5.2.1 (Alice), WBS.7.2.1 (Alex) | SS con fase 6 → gestione contenuti e prime view sponsor; riparte 09/04 post pausa |
| 8 | Sistema notifiche core | 26/05/2026 – 05/06/2026 | 14 | `▉▉▉` | WBS.6.1.* (Alice+Alex) | Dipende da eventi e admin → trigger utenti e preferenze |
| 9 | QA, performance, compliance | 08/06/2026 – 26/06/2026 | 20 | `▉▉▉▉` | WBS.8.1–8.5 (team) | FS da notifiche → test performance, crash, GDPR, accessibilità |
| 10 | Contenuti marketing, beta e store | 03/06/2026 – 30/06/2026 | 34 | `▉▉▉▉▉▉` | WBS.7.1.*, WBS.7.2.2, WBS.7.3.* | Overlap con QA (SS) → asset store, campagne social, beta interna, submission |

**Carico risorse:** la somma delle durate per fase replica i 177 gg eff. di R1 (2204). Alex concentra 230 h su front-end, filtri, marketing; Alice 281 h su backend/mobile, QA e store. Overlap intenzionale (fasi 6–10) per evitare tempi morti data la capacità limitata del team di 2 persone.

## Pianificazione R2 e R3
Release leggere gestite in “minisprint” di due settimane, mantenendo la stessa logica FS.

| Release | Sprint | Periodo | Durata (gg) | WBS coinvolti | Dipendenze e Deliverable |
|---|---|---|---|---|---|
| **R2** | S11 | 08/07/2026 – 21/07/2026 | 14 | WBS.3.1.*, WBS.3.2.1 | Richiede base R1 → data model coupon + CRUD gestori |
| | S12 | 22/07/2026 – 04/08/2026 | 13 | WBS.3.2.2, WBS.6.2.*, WBS.7.4.*, WBS.8.6.* | UI cliente, redemption, notifiche coupon, regression test, submission e comunicazione social |
| **R3** | S13 | 05/08/2026 – 18/08/2026 | 14 | WBS.4.1.*, WBS.4.2.1 | Definizione rating e modello recensioni |
| | S14 | 19/08/2026 – 01/09/2026 | 14 | WBS.4.2.2–4.3.1 | UI recensioni, moderazione, workflow segnalazioni |
| | S15 | 02/09/2026 – 15/09/2026 | 14 | WBS.4.3.2–4.3.3, WBS.6.3.1, WBS.7.4.*, WBS.8.6.* | Notifiche recensioni, regressione, submission e annuncio finale |

Le durate per R2 (41 gg) e R3 (56 gg) coincidono con le stime in 2204; ogni release mantiene 1 sprint per sviluppo feature e 1 sprint per integrazione+QA.

## Network Diagram R1
Per la rete logica usiamo nodi equivalenti ai pacchetti principali del Gantt. Le durate sono in giorni effettivi.

| Nodo | Durata (gg) | Attività (WBS) | Predecessori | Successori |
|---|---|---|---|---|
| N0 | 9 | Setup stack, auth base (5.1.1–5.1.2) | — | N1 |
| N1 | 10 | Modello dati + dataset locali (1.1.1–1.1.2) | N0 | N2 |
| N2 | 12 | CRUD locali + azioni rapide (1.1.3–1.1.4) | N1 | N3 |
| N3 | 23 | Mappa e geolocalizzazione (1.2.1–1.2.4) | N2 | N4 |
| N4 | 10 | Tipologie e filtri (1.3.1–1.3.2) | N3 | N5 |
| N5 | 32 | Sezione eventi (2.1–2.3) | N4 | N6 |
| N6 | 7 | Portale admin (5.2.1) | N5 | N7 |
| N7 | 14 | Notifiche (6.1.1–6.1.4) | N6 | N8 |
| N8 | 20 | QA/NFR (8.1–8.5) | N7 | N9 |
| N9 | 11 | Asset store + submission (7.1.1–7.1.2) | N8 | N10 |
| N10 | 13 | Sponsorizzazioni e campagne (7.2.*, 7.3.*) | N9 | N11 |
| N11 | 3 | Beta test + Go/No-Go (7.1.2, 7.3.3) | N10 | — |

### Critical Path
- **CP:** N0 → N1 → N2 → N3 → N4 → N5 → N6 → N7 → N8 → N9 → N11  
  (le attività marketing/sponsorizzazioni, N10, hanno slack di 2 gg perché possono terminare in parallelo al completamento QA).
- Durata complessiva CP ≈ 166 gg eff. → ~20 settimane + buffer (coerente con 2204).
- In termini di calendario equivale al periodo **01/12/2025 – 30/06/2026**, con le settimane 24/12–07/01 e 01/04–08/04 escluse dal conteggio.
- Slack principali: filtri eventi/liste (parte di N5) possiede 2 gg di galleggio, utilizzati per retesting dati; le attività social (7.3.1‑7.3.3) hanno 4 gg di slack e possono iniziare prima della fine di N8.

### Network R2/R3 (sintesi)
- R2 CP: Coupon data model → CRUD coupon → UI cliente → redemption → notifiche coupon → regression → submission (durata 41 gg). Nessun slack significativo: la submission (WBS.7.4.1) dipende dal completamento del flusso cliente.
- R3 CP: Configurazione punteggi → UI recensioni → moderazione → notifiche recensioni → regression → submission. Durata 56 gg con 3 gg di slack su comunicazione social.

## Governance e controllo
- Aggiornamento Gantt ogni sprint review; Earned Value semplice (planned vs actual hours) sfruttando le ore di 2204.
- Metriche di gating: completezza pacchetti WBS, difetti aperti < 5 prima dello store upload, checklist GDPR/Store (WBS.8.3.1 + 8.4.1) firmata.
- Il buffer di ~2 settimane tra fine sviluppo R1 e Go-Live copre i rischi catalogati in 2207 (store review, contenuti, carico team). R2 e R3 ereditano lo stesso schema con 2 gg di buffer interno per eventuali re-submit.
