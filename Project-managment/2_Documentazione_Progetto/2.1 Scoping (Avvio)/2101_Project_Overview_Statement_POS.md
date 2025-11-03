# 2101 — Project Overview Statement (POS) — CesenaLive

Scopo: autorizzazione iniziale del progetto pilota “CesenaLive”, app mobile per eventi/attività/locali a Cesena.

## Metadati
- Progetto: CesenaLive — App Città di Cesena
- Versione/Data: v1.0 / 2025‑02‑10
- Autori: Alex Siroli, Alice Mastrilli — Approver: Docente (Sponsor)

## 1) Problema / Opportunità
- Le informazioni su eventi, attività e locali a Cesena sono disperse tra molteplici canali; questo riduce visibilità e partecipazione.
- Opportunità: centralizzare l’offerta in un’unica app per incrementare partecipazione, spesa locale e attrattività turistica.

## 2) Goal del Progetto
- Realizzare e lanciare un MVP che consenta a cittadini/turisti di scoprire eventi e luoghi su mappa e calendario, con basi per estensioni future.

### 2.1 Value Proposition (discorsiva)
Per i cittadini e i turisti: un’unica app affidabile per scoprire cosa fare, senza cercare tra molteplici canali. Per gli esercenti: visibilità gratuita e strumenti semplici per promuovere eventi/offerte. Per la città: un hub digitale che favorisce partecipazione e spesa locale.

## 3) Obiettivi (SMART)
- Lanciare MVP su store in 10–12 settimane con ≥ 100 locali e ≥ 30 eventi/mese.
- Raggiungere MAU ≥ 500 a M2, rating medio ≥ 4.0 entro M2.
- Attivare ≥ 2 sponsorship locali entro M3.

## 4) Criteri di Successo (IRACIS)
- Increase Revenue: incremento spesa presso locali partner (proxy: redemption coupon ≥ 5%).
- Avoid Cost: riduzione tempo di ricerca informazioni (proxy: NPS ≥ 30).
- Improve Service: app unica con mappe/eventi/recensioni (proxy: retention D30 ≥ 20%).

## 5) Soluzione di Alto Livello e Alternative
- Soluzione: app mobile cross‑platform + backend API + admin portal; mappe e calendario; coupon e recensioni in release successive.
- Alternative: sito web mobile‑first; canali social aggregatori; scelta app per sfruttare geolocalizzazione, notifiche e store discoverability.

## 6) Ambito Iniziale e Out of Scope
- In scope (R1): mappa, eventi, schede locali base, admin minimo, analytics.
- R2: coupon/offerte; R3: recensioni/valutazioni.
- Out of scope (R1): pagamenti, moderazione community avanzata, machine learning di raccomandazione.

## 7) Assunzioni, Rischi e Ostacoli (alto livello)
- Assunzioni: contenuti forniti da esercenti/Comune; free tier mappe sufficiente; disponibilità canali promozionali locali.
- Rischi: bassa adozione, ritardi review store, carenza contenuti aggiornati, compliance GDPR.
- Ostacoli: tempo limitato del corso; risorse umane ridotte; dipendenze da provider.

## 8) Vincoli
- Tempo: 10–12 settimane per MVP; Budget: minimo (hosting/domino); Qualità: performance e stabilità; Compliance: GDPR, policy store.

## 9) Milestone Principali e Durata Stimata
- M1 PDS/WBS approvati (2025‑02‑10)
- M2 RC MVP pronta (settimana 8)
- M3 Rilascio store (settimana 10–12)

## 10) Budget Preliminare
- Costi vivi stimati: dominio 15€; hosting 10€/mese; mappe (free tier) 0€; strumenti 0€ (piani student).
- Valorizzazione ore interne (non a bilancio corso): ~300h a 25€/h = 7.500€ (solo per business case).

## 11) Stakeholder Principali
- Sponsor/Committente: Docente
- PM/Team: Alex Siroli, Alice Mastrilli
- Stakeholder: Comune di Cesena (potenziale partner), esercenti locali, cittadini/turisti, provider mappe, store Apple/Google.

## 12) Approvazioni
| Ruolo | Nome | Firma | Data |
|---|---|---|---|
| Sponsor | Docente del corso | — | 2025‑02‑10 |
| PM | Alex Siroli | — | 2025‑02‑10 |
| PM | Alice Mastrilli | — | 2025‑02‑10 |
### 5.1 Considerazioni architetturali
L’architettura privilegia componenti standard e servizi gestiti per contenere complessità (hosting managed, SDK mappe). La scelta mobile nativa/cross‑platform è guidata da requisiti di UX e time‑to‑market.
### 10.1 Note sulla sostenibilità
Il modello economico ipotizzato (sponsorship + ads) entra in gioco post‑MVP. Nella fase pilota, l’obiettivo è validare l’adozione minimizzando i costi vivi e massimizzando l’apprendimento.
