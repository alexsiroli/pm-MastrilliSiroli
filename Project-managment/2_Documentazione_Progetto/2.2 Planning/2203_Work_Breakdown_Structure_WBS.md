# 2203 — Work Breakdown Structure (WBS) — Ziradò

## RBS.1 — Mappa
La mappa orienta gli utenti nella città mostrando i luoghi più rilevanti con le relative schede.

### RBS.1.1 — Geolocalizzazione e posizionamento luoghi
- WBS.1.1.1 Raccolta e bonifica coordinate da fonti concordate.
- WBS.1.1.2 Indici geospaziali, validazioni e fallback di localizzazione.
- WBS.1.1.3 Test di accuratezza e monitoraggio (<50 m di media).

### RBS.1.2 — Schede locali
- WBS.1.2.1 Modello dati scheda (orari, servizi, menù, contatti).
- WBS.1.2.2 UI/UX scheda con stati vuoto/errore e caricamento.
- WBS.1.2.3 Azioni rapide: chiamata, navigazione mappa, condivisione.

### RBS.1.3 — Categorie/filtri
- WBS.1.3.1 Tassonomia tipologie con copertura 100% dei locali.
- WBS.1.3.2 API filtri (tipologia, prezzo, orari) con query indicizzate.
- WBS.1.3.3 UI filtri con persistenza selezioni e reset veloce.

## RBS.2 — Eventi
Sezione per eventi dei locali con vista elenco, calendario e scheda dettaglio.

### RBS.2.1 — Calendario e lista con filtri
- WBS.2.1.1 API lista eventi filtrabile per data/tipologia.
- WBS.2.1.2 UI calendario + lista con stati no‑result e loading.
- WBS.2.1.3 Ordinamento, paginazione e prestazioni su dataset ampi.

### RBS.2.2 — Dettaglio evento
- WBS.2.2.1 Modello evento (descrizione, location, orari, prezzo).
- WBS.2.2.2 UI dettaglio con deep‑link e condivisione.
- WBS.2.2.3 Validazioni e gestione contenuti mancanti.

### RBS.2.3 — Caricamento di eventi da gestori
- WBS.2.3.1 Form/Admin API per creazione/modifica evento.
- WBS.2.3.2 Pipeline di pubblicazione asincrona con SLA <5 minuti.
- WBS.2.3.3 Audit log e notifiche di esito al gestore.

## RBS.3 — Coupon/Offerte (R2)
Visualizzazione, creazione e uso di coupon con limiti configurabili.

### RBS.3.1 — Creazione/gestione coupon da parte dei gestori
- WBS.3.1.1 Modello coupon (descrizione, limiti, validità).
- WBS.3.1.2 UI/Admin gestione coupon e report base.
- WBS.3.1.3 Pubblicazione asincrona con visibilità entro 5 minuti.

### RBS.3.2 — Utilizzo del coupon da parte dei clienti
- WBS.3.2.1 Flusso redeem in app con feedback chiaro sugli errori.
- WBS.3.2.2 Regole limiti per utente e idempotenza delle richieste.
- WBS.3.2.3 Log utilizzi e prevenzione abusi (rate‑limit/anti‑fraud).

## RBS.4 — Recensioni (R3)
Valutazioni e recensioni con moderazione base.

### RBS.4.1 — Valutazioni per tipologia di locale
- WBS.4.1.1 Definizione di ≥5 criteri per tipologia.
- WBS.4.1.2 UI rating e persistenza delle risposte.
- WBS.4.1.3 Analisi base dei punteggi per locale.

### RBS.4.2 — Recensioni testuali
- WBS.4.2.1 Invio recensione con convalida e anti‑spam.
- WBS.4.2.2 UI composizione con limiti testo e messaggi guida.
- WBS.4.2.3 Salvataggio affidabile e gestione errori di rete.

### RBS.4.3 — Moderazione base
- WBS.4.3.1 Coda segnalazioni e vista moderazione.
- WBS.4.3.2 Azioni approva/oscura con motivazioni e log.
- WBS.4.3.3 Esposizione solo recensioni approvate.

## RBS.5 — Backend/API e Admin
Infrastruttura, sicurezza e pannello amministrativo.

### RBS.5.1 — Autorizzazione in base al ruolo
- WBS.5.1.1 Login e gestione token (JWT/OAuth).
- WBS.5.1.2 Ruoli e permessi RBAC sugli endpoint sensibili.
- WBS.5.1.3 Audit log delle operazioni amministrative.

### RBS.5.2 — Interfaccia per amministratore
- WBS.5.2.1 CRUD luoghi/eventi con validazioni e upload media.
- WBS.5.2.2 Import/export massivo e calendari operativi.
- WBS.5.2.3 Moderazione recensioni e usabilità back‑office.

## RBS.6 — Sistema di Notifiche
Notifiche su eventi/offerte/aggiornamenti con preferenze utente.

### RBS.6.1 — Notifiche
- WBS.6.1.1 Gestione token push iOS/Android e preferenze utente.
- WBS.6.1.2 Invii per topic/evento/offerta e deep‑link.
- WBS.6.1.3 Test ricezione su ≥5 device e dashboard invii.

## RBS.7 — Requisiti Non Funzionali
Qualità, privacy e conformità trasversali.

### RBS.7.1 — Performance
- WBS.7.1.1 Profiling viste core e budget P95 <2s.
- WBS.7.1.2 Ottimizzazioni query/API e caching mirato.
- WBS.7.1.3 Monitoraggio continuo e regressioni performance.

### RBS.7.2 — Stabilità
- WBS.7.2.1 Crash reporting integrato e alerting.
- WBS.7.2.2 Hardening errori critici e retry policy.
- WBS.7.2.3 Test resilienza su scenari di rete.

### RBS.7.3 — Privacy/GDPR (consensi, policy)
- WBS.7.3.1 Raccolta consensi, registro eventi e revoca.
- WBS.7.3.2 Policy chiare in‑app e minimizzazione dati.
- WBS.7.3.3 Gestione diritti (accesso/cancellazione) e DPA.

### RBS.7.4 — Rispetto delle normative degli store
- WBS.7.4.1 Checklist Apple/Google e adeguamenti.
- WBS.7.4.2 Verifiche pre‑submission e superamento validazioni.
- WBS.7.4.3 Gestione feedback revisione e hotfix.

### RBS.7.5 — Accessibilità base
- WBS.7.5.1 Contrasti, label e ruoli semantici.
- WBS.7.5.2 Navigazione assistiva e dimensioni testo adattive.
- WBS.7.5.3 Test WCAG 2.1 AA sulle viste core.
