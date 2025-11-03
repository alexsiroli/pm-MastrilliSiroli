# 2202 — Requirements Breakdown Structure (RBS) — CesenaLive

Scopo: scomporre i requisiti in modo gerarchico per mappa, eventi, coupon e recensioni, inclusi NF e vincoli.

## Convenzioni
- Codifica ID: RBS.X.Y (X livello, Y progressivo)
- Categorie: F = Funzionali, NF = Non funzionali, C = Vincoli

## Struttura
```
RBS.1 Mappa (F)
  RBS.1.1 Geolocalizzazione e posizionamento luoghi (F)
  RBS.1.2 Categorie/filtri (F)
  RBS.1.3 Schede locali (info base: orari, servizi, contatti) (F)
RBS.2 Eventi (F)
  RBS.2.1 Calendario e lista con filtri (F)
  RBS.2.2 Dettaglio evento (descrizione, luogo, orari, prezzo) (F)
  RBS.2.3 Submission eventi da gestori/cittadini (moderazione minima) (F)
RBS.3 Coupon/Offerte (F, R2)
  RBS.3.1 Creazione/gestione coupon da parte dei gestori (F)
  RBS.3.2 Redemption e tracking (F)
RBS.4 Recensioni (F, R3)
  RBS.4.1 Valutazioni per tipologia locale/esperienza (F)
  RBS.4.2 Moderazione base (F)
RBS.5 Backend/API e Admin (F)
  RBS.5.1 API REST sicure (F)
  RBS.5.2 Admin portal minimo (F)
RBS.6 Analytics e Notifiche (F)
  RBS.6.1 Analytics base (F)
  RBS.6.2 Notifiche (opzionale) (F)
RBS.7 Requisiti Non Funzionali (NF)
  RBS.7.1 Performance P95 < 2s viste principali (NF)
  RBS.7.2 Stabilità crash/sessione < 1% (NF)
  RBS.7.3 Privacy/GDPR (consensi, policy) (NF)
  RBS.7.4 Accessibilità base (NF)
RBS.8 Vincoli (C)
  RBS.8.1 Policy store Apple/Google (C)
  RBS.8.2 Budget minimo e tempo corso (C)
```

## Tabella di Riferimento
| ID | Titolo | Tipo | Descrizione | Criteri di Accettazione | Fonte | Note |
|---|---|---|---|---|---|---|
| RBS.1.1 | Geolocalizzazione | F | Mostrare luoghi su mappa | Marker corretti su 3 device | Utenti | MVP |
| RBS.2.1 | Calendario eventi | F | Lista/filtri | Ricerca per data/categoria | Utenti | MVP |
| RBS.3.1 | Coupon gestori | F | Creazione offerte | Redemption tracciata | Esercenti | R2 |
| RBS.7.3 | GDPR | NF | Consenso/privacy | Policy visibile/consenso raccolto | Compliance | MVP |

### Note discorsive
La RBS è raccontata in funzione dell’esperienza utente: il flusso “scopro → valuto → mi muovo” parte da mappa/lista e si conclude in dettaglio evento/luogo. La raccolta di feedback guiderà l’evoluzione delle categorie e dei filtri. I requisiti non funzionali (performance, stabilità, privacy) sono esplicitati perché determinanti per l’approvazione store e la soddisfazione degli utenti.
