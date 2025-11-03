# 2401 — Project Status Report — CesenaLive (Esempio)

Scopo: comunicazione periodica sullo stato con indicatori, scostamenti e azioni.

## Intestazione
| Campo | Valore |
|---|---|
| Data | 2025‑03‑01 |
| Periodo coperto | Settimane 1–2 |
| Stato complessivo | Giallo |
| PM | Alex Siroli / Alice Mastrilli |

## Executive Summary
Setup backend/DB completato; API luoghi al 60%; shell app e mappa prototipale al 40%. Leggero ritardo su API eventi per imprevisto DB.

## Avanzamento per Deliverable/Task
| ID | Nome | % Completato | Note |
|---|---|---|---|
| WBS.3.1 | Setup backend/DB | 100% | Concluso |
| WBS.3.2 | API Luoghi | 60% | In corso |
| WBS.3.3 | API Eventi | 30% | In ritardo di 2gg |
| WBS.4.1 | Shell/navigazione | 80% | Quasi completo |
| WBS.4.2 | Vista mappa | 40% | Prototype ok |

## Scostamenti Principali e Cause
- Tempo: −2gg su API Eventi per schema DB rivisto; mitigazione: pairing e focus.

## KPI (EVA)
| PV | EV | AC | SV | CV | SPI | CPI |
|---|---|---|---|---|---|---|
| 80 | 70 | 85 | −10 | −15 | 0,88 | 0,82 |

## Rischi / Issues Top
| Tipo | ID | Descrizione | Impatto | Owner | Stato |
|---|---|---|---|---|---|
| Rischio | RSK‑002 | Ritardo review store | Medio | Alex | Aperto |
| Issue | ISS‑001 | Crash dettaglio evento | Alto | Alice | In corso |

## Azioni Correttive / Prossime Settimane
- Focus su API Eventi; integrare mappa; preparare test plan; avvio outreach esercenti.

### Note d’uso del report
Compilare lo status con dati oggettivi (commit, ticket chiusi, tempo speso) e metriche chiare (PV, EV, AC). Limitare il testo a evidenze e decisioni necessarie; rimandare i dettagli al board.
