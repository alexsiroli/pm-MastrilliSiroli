# 2402 — Project Impact Statement — CesenaLive (Esempio)

Scopo: analizzare l’impatto della SCR‑001 (login social) su R1.

## Riferimenti
- ID Scope Change Request: SCR‑001
- Link valutazioni: 2303, note tecniche repository

## Impatto Valutato
| Dimensione | Situazione Attuale | Impatto della Modifica | Note |
|---|---|---|---|
| Tempo | Rilascio R1 in sett. 10–12 | +5–8 gg | Prop. spostare a R2 |
| Costi | Vivi ~65€; ore interne baseline | +32–48h | Non a bilancio corso |
| Qualità | MVP stabile | Migliora UX | Aumenta superfici test |
| Risorse | 0,5+0,5 FTE | Picco extra | Richiede pianificazione |

## Opzioni Considerate
- A: Integrare in R1 (pro: UX; contro: rischio CP)
- B: Spostare a R2 (pro: protegge CP; contro: valore posticipato)

## Raccomandazione del PM
- Opzione B: spike 1g in R1 e implementazione completa in R2.

## Valutazione Rischio
- Rischio store/GDPR; mitigazioni definite in 2208.

## Approvazioni
| Ruolo | Nome | Decisione | Firma | Data |
|---|---|---|---|---|
| Sponsor | Docente | Approvato | — | 2025‑02‑19 |
| PM | Alex/Alice | Allineati | — | 2025‑02‑19 |

### Nota metodologica
L’impact statement deve rendere espliciti i trade‑off. Se un’opzione migliora UX ma mette a rischio il cammino critico, si propone un approccio in due tempi (spike in R1, feature in R2) per proteggere la delivery del MVP.
