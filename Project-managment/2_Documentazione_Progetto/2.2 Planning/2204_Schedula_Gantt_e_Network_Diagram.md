# 2204 — Schedula Gantt e Network Diagram — Ziradò

Scopo: definire sequenze, dipendenze e tempi attività R1, con CP atteso Backend→Mobile→QA→Store.

## Sequenziamento e Dipendenze
- Tipi: FS prevalente; qualche SS per design/UI e content.
- Calendario: 5g/sett, 20h/sett per persona; sprint 2 settimane.

## Tabella Attività (Estratto R1)
| ID | Nome | Durata | Dipendenze | ES | EF | LS | LF | Float |
|---|---|---|---|---|---|---|---|---|
| WBS.3.1 | Setup backend/DB | 3g | — | D1 | D3 | D1 | D3 | 0 |
| WBS.3.2 | API Luoghi | 4g | WBS.3.1 (FS) | D4 | D7 | D4 | D7 | 0 |
| WBS.3.3 | API Eventi | 4g | WBS.3.1 (FS) | D4 | D7 | D4 | D7 | 0 |
| WBS.4.1 | Shell/navigazione app | 3g | WBS.2.1 (SS) | D4 | D6 | D6 | D8 | 2 |
| WBS.4.2 | Vista mappa | 5g | WBS.3.2 (FS) | D8 | D12 | D8 | D12 | 0 |
| WBS.4.3 | Lista/filtri eventi | 4g | WBS.3.3 (FS) | D8 | D11 | D10 | D13 | 2 |
| WBS.4.4 | Dettagli | 3g | WBS.4.2/4.3 (FS) | D13 | D15 | D13 | D15 | 0 |
| WBS.7.1 | Test plan/smoke | 2g | WBS.4.4 (FS) | D16 | D17 | D16 | D17 | 0 |
| WBS.7.2 | Beta test | 3g | WBS.7.1 (FS) | D18 | D20 | D18 | D20 | 0 |
| WBS.7.3 | Submission store | 3g | WBS.7.2 (FS) | D21 | D23 | D21 | D23 | 0 |

Note: Dn = giorno lavorativo n dalla partenza R1.

## Critical Path
- CP: WBS.3.1 → WBS.3.2 → WBS.4.2 → WBS.4.4 → WBS.7.1 → WBS.7.2 → WBS.7.3

### Narrazione di schedulazione
La sequenza riflette la natura dipendente delle feature core: senza API luoghi affidabili, la mappa non può essere completata; senza mappa e dettagli eventi, i test di sistema non hanno valore. Il buffer pre‑store consente remediation rapida di eventuali punti deboli emersi in beta.

## Allegati/Link
- Diagrammi esportati in seguito alla definizione puntuale con tool Gantt.
