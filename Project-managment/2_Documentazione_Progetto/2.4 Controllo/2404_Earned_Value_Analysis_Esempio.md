# 2404 — Earned Value Analysis (Esempio) — CesenaLive

Scopo: calcolare PV, EV, AC e indici SPI/CPI su sprint iniziali R1.

## Dati Esempio (Settimane 1–2, unità: ore)
| Attività | PV | EV | AC |
|---|---|---|---|
| WBS.3.1 Setup backend/DB | 20 | 20 | 22 |
| WBS.3.2 API Luoghi | 16 | 12 | 14 |
| WBS.4.1 Shell app | 12 | 10 | 11 |
| Totale | 48 | 42 | 47 |

## Calcoli
- SV = EV − PV = 42 − 48 = −6 (in ritardo)
- CV = EV − AC = 42 − 47 = −5 (oltre costo/effort)
- SPI = EV / PV = 0,88
- CPI = EV / AC ≈ 0,89

## Proiezioni (esempio)
- BAC (effort R1) = 300h; con CPI=0,89 → EAC ≈ 337h (azione correttiva necessaria per rientrare).
- ETC = EAC − AC_cumulato.

Nota: rivedere stime o priorità per recuperare SPI/CPI ≥ 0,95.

### Scelte metodologiche (discorsive)
EAC può essere stimato in più modi: (1) BAC/CPI quando il trend di costo permane; (2) AC + (BAC − EV) quando si assume CPI=1 per il lavoro restante; (3) AC + (BAC − EV)/(CPI×SPI) quando ritardi e sforamenti coesistono. Qui si privilegia la variante prudente (1) per anticipare azioni correttive.
