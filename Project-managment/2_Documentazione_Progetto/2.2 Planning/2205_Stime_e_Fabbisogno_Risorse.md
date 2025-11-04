# 2205 — Stime e Fabbisogno Risorse — Ziradò

Scopo: stimare effort/durata e definire il fabbisogno di risorse per R1.

## Metodi di Stima
- Three‑Point (O/M/P); assunzioni: 20h/sett persona; rischio buffer 10% su CP.

## Tabella Stime per Attività (Estratto)
| ID | Nome | Effort O/M/P (h) | Durata O/M/P (g) | Ruolo | Skill | Note |
|---|---|---|---|---|---|---|
| WBS.3.1 | Setup backend/DB | 16/20/28 | 2/3/4 | Dev (Alex) | API/DB | — |
| WBS.3.2 | API Luoghi | 20/24/32 | 3/4/5 | Dev (Alex) | API | — |
| WBS.4.2 | Vista mappa | 24/32/40 | 3/4/5 | Dev (Alice) | Mobile/Map | Dip. WBS.3.2 |
| WBS.4.3 | Lista eventi | 16/24/32 | 2/3/4 | Dev (Alice) | Mobile | Dip. WBS.3.3 |
| WBS.7.3 | Submission store | 12/16/24 | 2/3/4 | PM/Dev (Alex) | Store | — |

## Fabbisogno Complessivo (Sintesi)
| Ruolo | FTE/mesi | Periodo | Vincoli |
|---|---|---|---|
| PM/Dev Alex | 0,5 | M1–M3 | Esami/sessioni |
| Dev/UX Alice | 0,5 | M1–M3 | Esami/sessioni |

### Note discorsive
Le stime considerano finestre di studio/esami: si adottano sprint realistici, WIP limitato e pairing su task critici. La capacità ridotta è compensata da scelte tecnologiche pragmatiche e da un perimetro di MVP rigoroso.
