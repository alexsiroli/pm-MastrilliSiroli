# 2208 — Analisi Rischi e Mitigazione — CesenaLive

Scopo: identificare, valutare e trattare rischi su adozione, contenuti, store, compliance e capacità.

## Matrice del Rischio
- Scala: Probabilità 1–5; Impatto 1–5; Priorità = P×I.

## Registro Rischi
| ID | Descrizione | Categoria | Prob. | Impatto | Priorità | Strategia | Trigger | Owner | Mitigazione | Contingenza | Residuo | Stato |
|---|---|---|---|---|---|---|---|---|---|---|---|---|
| RSK‑001 | Bassa adozione utenti | PM | 3 | 4 | 12 | M | MAU <60% target | Alice | Outreach esercenti, UX simpl. | Sprint growth | Medio | Aperto |
| RSK‑002 | Ritardo review store | Esterno | 2 | 5 | 10 | A | Review >7gg | Alex | Preparare linee guida | Buffer 2 sett. | Basso | Aperto |
| RSK‑003 | Contenuti non aggiornati | Org | 4 | 3 | 12 | M | <30 eventi/mese | Alice | Onboarding esercenti | Curare scraping lecito | Medio | Aperto |
| RSK‑004 | Violazioni GDPR | Compliance | 2 | 5 | 10 | T | Reclami/privacy | Alex | Minimizzazione dati | Disatt. feature | Basso | Aperto |
| RSK‑005 | Sovraccarico team | PM | 3 | 3 | 9 | M | Slittamenti CP | Alex | WIP limit, focus CP | Ridurre scope | Medio | Aperto |

Strategia: M=Mitigate, A=Avoid, T=Transfer, Acc=Accept

## Riesame Periodico
- Revisione settimanale; chiusura quando trigger assente per 4 settimane o mitigazione consolidata.

### Interpretazione heatmap (discorsiva)
I rischi ad alta priorità (rossi) richiedono azione preventiva immediata (es. buffer store review). I medi (arancioni) si tengono monitorati con trigger chiari (es. KPI di adozione). I bassi (verdi) si accettano, rivalutandoli a ogni milestone.
