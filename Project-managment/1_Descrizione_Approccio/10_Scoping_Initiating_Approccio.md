# 10 — Scoping/Initiating: Approccio (Ziradò)

Scopo: definire confini, condizioni di soddisfazione e requisiti high‑level per l’avvio del progetto pilota a Cesena.

## 1) Obiettivi dello Scoping
- Esplicitare problema/opportunità: informazioni frammentate su eventi/attività/luoghi, basso coinvolgimento.
- Definire CoS e criteri di accettazione per MVP (R1) e release successive (R2, R3).
- Raccogliere requisiti high‑level e allineare sponsor, stakeholder locali e team.

## 2) Conditions of Satisfaction (CoS)
- Pubblicazione MVP su store in 10–12 settimane, in area Cesena.
- Funzionalità minime R1: mappa interattiva, calendario eventi con filtri, schede locali base, submission eventi, backend admin minimo.
- Qualità: performance P95 < 2s su principali viste; crash rate < 1%/sessione; UX semplice.
- Dati: ≥ 100 locali, ≥ 30 eventi/mese al lancio; aggiornamento contenuti settimanale.
- Compliance: GDPR (privacy policy, consenso), policy store (review guidelines), accessibilità WCAG considerata.
- Metriche d’adozione: MAU ≥ 500 a M2; rating ≥ 4.0.

Verifica: demo interna, beta (TestFlight/closed track), checklist store, smoke test su 3 device target.

## 3) Requisiti di Alto Livello (RBS – livello 1)
- F1 Mappa interattiva di luoghi/attività (geoloc, categorie, orari, servizi).
- F2 Area eventi con calendario, filtri, dettagli, condivisione.
- F3 Coupon/offerte speciali attivabili dai gestori (R2).
- F4 Sistema recensioni (per tipologia locale e esperienza) (R3).
- F5 Backend/API e admin portal essenziale; F6 Onboarding contenuti; F7 Analytics.
- NF1 Prestazioni; NF2 Privacy/GDPR; NF3 Accessibilità; NF4 Affidabilità; C1 Policy store; C2 Budget/tempo.

Tracciabilità: POS → RBS; RBS → WBS (2203).

### 3.1 Personas e Job‑to‑Be‑Done (discorsivo)
- Persona “Cittadina Curiosa”: vuole scoprire in pochi tocchi cosa succede nel weekend; JTBD: “Quando ho un’ora libera, voglio trovare un evento vicino e adatto alle mie preferenze, così da non perdere tempo a cercare su più canali”.
- Persona “Esercente Proattivo”: desidera promuovere serate e offerte; JTBD: “Voglio pubblicare un evento e un coupon da un’unica interfaccia semplice e ottenere visibilità misurabile”.
Queste personas guidano priorità e UX (filtri chiari, mappa veloce, submission snella).

## 4) POS: Sintesi e Approvazione
- Vedi `2.1 Scoping (Avvio)/2101_Project_Overview_Statement_POS.md`.
- Autorità di approvazione: Sponsor/Committente (Docente), PM (Alex Siroli, Alice Mastrilli).
- Criteri ingresso planning: CoS confermate; RBS L1/L2 definita; rischio preliminare classificato.

## 5) Rischi Iniziali e Stakeholder
- Rischi top: bassa adozione; contenuti non aggiornati; ritardi store; privacy; capacità team.
- Stakeholder iniziali: cittadini, esercenti, Comune, sponsor (Docente), partner potenziali.

## 6) Uscite/Artefatti
- POS approvato, CoS definite, RBS L1/L2 abbozzata, elenco assunzioni.

## 7) Checklist
- [x] CoS definiti e condivisi
- [x] Requisiti high‑level documentati
- [x] POS bozza approvata
- [x] Rischi iniziali identificati

### 8) Narrazione dello scoping
Lo scoping ha chiarito che il valore del MVP dipende dalla facilità con cui gli utenti trovano informazioni affidabili e aggiornate. Per questo, la submission eventi deve essere semplice per i gestori, e il dataset iniziale di luoghi va curato manualmente (seed) per garantire qualità. La scelta di rinviare a R2 i coupon e a R3 le recensioni mantiene il focus sul “discoverability” e riduce la complessità in fase di avvio.
