# 2203 — Work Breakdown Structure (WBS) — Ziradò

## Struttura
```
WBS.1 Project Management
  WBS.1.1 Pianificazione e JPPS
  WBS.1.2 Monitoraggio e report
  WBS.1.3 Chiusura
WBS.2 UX/UI
  WBS.2.1 Wireframe mappa/eventi
    WBS.2.1.1 Personas e user journey principali
    WBS.2.1.2 Wireframe low‑fi (mappa, lista, dettaglio luogo/evento)
    WBS.2.1.3 Flussi: filtri, ricerca, redeem coupon, recensione
  WBS.2.2 UI componenti principali
    WBS.2.2.1 Design system (colori, tipografia, spaziature)
    WBS.2.2.2 Componenti: card luogo, card evento, chip filtri
    WBS.2.2.3 Stati vuoto/errore/loading
  WBS.2.3 Store listing (screenshot, descrizioni)
WBS.3 Backend/API
  WBS.3.1 Setup progetto e DB
    WBS.3.1.1 Scaffolding repo e ambienti (dev/stage/prod)
    WBS.3.1.2 Modello dati base (luoghi, categorie, eventi, utenti, ruoli)
    WBS.3.1.3 CI di base (build, test)
  WBS.3.2 Servizi Luoghi (geo, categorie)
    WBS.3.2.1 Schema luoghi: campi geo + indici
    WBS.3.2.2 Endpoint CRUD luoghi
    WBS.3.2.3 Ricerca/filtri (categoria, prezzo, orari)
    WBS.3.2.4 Import iniziale (supporto CSV/Sheet)
  WBS.3.3 Servizi Eventi (lista, dettaglio)
    WBS.3.3.1 Modello evento (fascia oraria, prezzo, location)
    WBS.3.3.2 API lista con filtri + calendario
    WBS.3.3.3 API dettaglio evento
    WBS.3.3.4 Pubblicazione asincrona (<5m) con coda job
  WBS.3.4 Autenticazione/Autorizzazioni (RBAC) + Audit log
    WBS.3.4.1 Login e token (JWT/OAuth)
    WBS.3.4.2 Ruoli: admin, gestore, utente
    WBS.3.4.3 Middleware autorizzazioni per endpoint sensibili
    WBS.3.4.4 Audit log azioni
  WBS.3.5 Notifiche (topic, push gateway)
    WBS.3.5.1 Gestione token push iOS/Android
    WBS.3.5.2 Preferenze notifiche per utente
    WBS.3.5.3 Invio per topic/evento/offerta
    WBS.3.5.4 Webhook test + dashboard invii
  WBS.3.6 Servizi Coupon (crea/gestisci/usa)
    WBS.3.6.1 Modello coupon (descrizione, limiti, validità)
    WBS.3.6.2 API creazione/gestione coupon
    WBS.3.6.3 API redeem con limiti per utente
    WBS.3.6.4 Anti‑fraud base (idempotenza, rate‑limit)
  WBS.3.7 Servizi Recensioni (rating, testo, segnalazioni)
    WBS.3.7.1 Modello rating per tipologia di locale
    WBS.3.7.2 API invio recensione (rating + testo)
    WBS.3.7.3 Segnalazione recensioni
    WBS.3.7.4 Anti‑spam base (throttling)
  WBS.3.8 Moderazione recensioni (stati, workflow)
    WBS.3.8.1 Stati: in revisione, approvata, oscurata
    WBS.3.8.2 Azioni admin + log motivazioni
    WBS.3.8.3 Esposizione solo recensioni approvate
WBS.4 Mobile App
  WBS.4.1 Shell app, navigazione
    WBS.4.1.1 Setup progetti iOS/Android
    WBS.4.1.2 Navigazione tab/stack
    WBS.4.1.3 Gestione stato e storage locale
  WBS.4.2 Vista mappa e marker (geoloc)
    WBS.4.2.1 Permessi location e fallback
    WBS.4.2.2 Render mappa (tile, clustering)
    WBS.4.2.3 Marker e schede luogo
  WBS.4.3 Lista/filtri eventi e luoghi
    WBS.4.3.1 UI filtri (categoria, prezzo, orari)
    WBS.4.3.2 Ricerca testuale
    WBS.4.3.3 Stati vuoto e no‑result
  WBS.4.4 Dettaglio evento/luogo
    WBS.4.4.1 Dati principali e contatti
    WBS.4.4.2 Orari/aperture e prezzi
    WBS.4.4.3 Deep‑link da notifica
  WBS.4.5 Analytics base
    WBS.4.5.1 Eventi: aperture vista, click marker, redeem
    WBS.4.5.2 Dashboard minima
  WBS.4.6 Coupon: lista/dettaglio/riscatto
    WBS.4.6.1 Lista coupon disponibili
    WBS.4.6.2 Dettaglio e condizioni
    WBS.4.6.3 Flusso redeem + feedback errore
  WBS.4.7 Recensioni: rating, testo, segnalazione
    WBS.4.7.1 UI rating per tipologia
    WBS.4.7.2 Testo e invio
    WBS.4.7.3 Segnalazione recensione
  WBS.4.8 Notifiche: opt‑in, preferenze, deep‑link
    WBS.4.8.1 Opt‑in e permessi
    WBS.4.8.2 Preferenze utente
    WBS.4.8.3 Deep‑link verso viste
WBS.5 Admin Portal
  WBS.5.1 CRUD luoghi
    WBS.5.1.1 Form e validazioni
    WBS.5.1.2 Upload media
    WBS.5.1.3 Import bulk
  WBS.5.2 CRUD eventi (pubblicazione <5m)
    WBS.5.2.1 Creazione/modifica
    WBS.5.2.2 Pubblicazione asincrona <5m
    WBS.5.2.3 Calendario e filtri
  WBS.5.3 Gestione coupon
    WBS.5.3.1 Configurazione limiti e validità
    WBS.5.3.2 Report utilizzi
  WBS.5.4 Moderazione recensioni
    WBS.5.4.1 Coda segnalazioni
    WBS.5.4.2 Azioni approva/oscura
  WBS.5.5 Gestione ruoli e permessi
    WBS.5.5.1 Assegnazione ruoli
    WBS.5.5.2 Gestione inviti/utenti
WBS.6 Content Onboarding
  WBS.6.1 Raccolta dati luoghi
    WBS.6.1.1 Sorgenti e formati
    WBS.6.1.2 Normalizzazione e qualità
  WBS.6.2 Calendario eventi iniziale
    WBS.6.2.1 Contatto gestori
    WBS.6.2.2 Popolamento seed
  WBS.6.3 Tassonomia categorie/filtri (copertura 100%)
    WBS.6.3.1 Definizione tassonomia
    WBS.6.3.2 Copertura 100% tipologie
WBS.7 QA & Release
  WBS.7.1 Test plan e smoke test
    WBS.7.1.1 Casi d’uso prioritari RBS
    WBS.7.1.2 E2E notifiche su 5 device
  WBS.7.2 Beta TestFlight/Closed Track
    WBS.7.2.1 Distribuzione build
    WBS.7.2.2 Raccolta feedback
  WBS.7.3 Submission store
    WBS.7.3.1 Checklist store
  WBS.7.4 Test performance e stabilità (NFR)
    WBS.7.4.1 Profiling P95 viste core
    WBS.7.4.2 Crash reporting <1%
  WBS.7.5 Privacy/GDPR: consensi, policy
    WBS.7.5.1 Consensi espliciti e log
    WBS.7.5.2 Policy e data minimization
  WBS.7.6 Accessibilità base (WCAG 2.1 AA)
    WBS.7.6.1 Contrasti e label
    WBS.7.6.2 Navigazione assistiva
  WBS.7.7 Conformità linee guida store
    WBS.7.7.1 Requisiti specifici Apple/Google
WBS.8 Growth/Marketing
  WBS.8.1 Landing e materiali promo
  WBS.8.2 Outreach esercenti
```

## Allineamento RBS → WBS
- RBS.1 Mappa → `WBS.3.2`, `WBS.4.2`, `WBS.2.1`, `WBS.6.3`
- RBS.1.1 Geolocalizzazione → `WBS.3.2` (campi geo + indici), `WBS.4.2` (permessi/location + marker)
- RBS.1.2 Schede locali → `WBS.3.2` (endpoint dettaglio), `WBS.4.4` (UI dettaglio luogo), `WBS.5.1` (contenuti)
- RBS.1.3 Categorie/filtri → `WBS.3.2` (modello categorie), `WBS.4.3` (UI filtri), `WBS.6.3` (tassonomia)
- RBS.2 Eventi → `WBS.3.3`, `WBS.4.3`, `WBS.4.4`, `WBS.5.2`
- RBS.2.1 Calendario/lista con filtri → `WBS.3.3`, `WBS.4.3`
- RBS.2.2 Dettaglio evento → `WBS.3.3`, `WBS.4.4`
- RBS.2.3 Caricamento eventi da gestori → `WBS.5.2` (CRUD + publish), `WBS.3.3` (pipeline), SLA < 5 min: `WBS.7.1`
- RBS.3 Coupon/Offerte (R2) → `WBS.3.6`, `WBS.4.6`, `WBS.5.3`, `WBS.7.1`
- RBS.3.1 Creazione/gestione coupon (gestori) → `WBS.5.3`, `WBS.3.6`
- RBS.3.2 Utilizzo coupon (clienti) → `WBS.4.6`, `WBS.3.6` (limiti d’uso)
- RBS.4 Recensioni (R3) → `WBS.3.7`, `WBS.4.7`, `WBS.5.4`, `WBS.3.8`
- RBS.4.1 Valutazioni per tipologia → `WBS.3.7` (schema dinamico), `WBS.4.7` (UI per tipologia)
- RBS.4.2 Recensioni testuali → `WBS.3.7`, `WBS.4.7`
- RBS.4.3 Moderazione base → `WBS.3.8`, `WBS.5.4`
- RBS.5 Backend/API e Admin → `WBS.3.*`, `WBS.5.*` con focus su `WBS.3.4` (RBAC, audit)
- RBS.5.1 Autorizzazione per ruolo → `WBS.3.4`, `WBS.5.5`
- RBS.5.2 Interfaccia amministratore → `WBS.5.*`
- RBS.6 Sistema di Notifiche → `WBS.3.5`, `WBS.4.8`, `WBS.7.1`
- RBS.6.1 Notifiche → `WBS.3.5` (backend), `WBS.4.8` (preferenze, deep‑link), test multi‑device: `WBS.7.1`
- RBS.7 Requisiti Non Funzionali → `WBS.7.4` (performance, stabilità), `WBS.7.5` (privacy/GDPR), `WBS.7.6` (accessibilità), `WBS.7.7` (store)

## Dizionario WBS (Estratto)
| ID | Nome | Descrizione | Output | Criteri di Completamento | Dipendenze | Effort (O/M/P) | Durata (O/M/P) | Owner |
|---|---|---|---|---|---|---|---|---|
| WBS.3.2 | Servizi Luoghi | API CRUD luoghi (geo, filtri) | Endpoint v1 | Test unit + doc | WBS.3.1 | 10/12/16h | 2/3/4g | Alex |
| WBS.4.2 | Vista mappa | UI mappa + marker | Vista funzionante | P95<2s, 3 device | WBS.3.2 | 12/16/20h | 3/4/5g | Alice |
| WBS.3.3 | Servizi Eventi | API lista/calendario/dettaglio | Endpoint v1 | Test integrazione base | WBS.3.1 | 10/14/18h | 2/3/4g | Alex |
| WBS.5.2 | CRUD eventi | Admin crea/modifica/pubblica | Evento online | SLA publish <5 min | WBS.3.3 | 8/12/16h | 2/3/4g | Alice |
| WBS.3.5 | Notifiche backend | Gateway + topic + API | Notifica test inviata | 5 device ricevono | WBS.3.1 | 8/12/16h | 2/3/4g | Alex |
| WBS.4.8 | Notifiche app | Opt‑in, preferenze, deep‑link | UI + storage | 3 scenari E2E ok | WBS.3.5 | 8/12/16h | 2/3/4g | Alice |
| WBS.3.6 | Servizi Coupon | CRUD coupon + redeem | Endpoint v1 | Limite usi rispettato | WBS.3.1 | 10/14/18h | 2/3/4g | Alex |
| WBS.4.6 | UI Coupon | Lista/dettaglio/riscatto | Flusso redeem | 3 device, errori gestiti | WBS.3.6 | 10/14/18h | 2/3/4g | Alice |
| WBS.3.7 | Servizi Recensioni | Rating + testo + report | Endpoint v1 | Anti‑spam base | WBS.3.1 | 10/14/18h | 2/3/4g | Alex |
| WBS.5.4 | Moderazione recensioni | Approva/oscura segnalate | UI + azioni | SLA moderazione 1g | WBS.3.8 | 6/10/14h | 2/3/4g | Alice |
| WBS.7.4 | Test performance | Profila e ottimizza viste core | Report P95 | P95<2s, crash<1% | WBS.4.* | 8/12/16h | 2/3/4g | Alex |
| WBS.7.5 | Privacy/GDPR | Consensi, policy, minimizzazione | Flusso consensi | Policy visibile, log | WBS.4.1 | 6/10/14h | 2/3/4g | Alex |
| WBS.7.6 | Accessibilità | Contrasti, label, navigazione | Checklist WCAG | AA sulle viste core | WBS.2.* | 6/8/12h | 2/3/4g | Alice |
| WBS.7.3 | Submission store | Requisiti store | App inviata | Checklist store ok | WBS.7.2 | 6/8/12h | 2/3/4g | Alex |
| WBS.3.4.1 | Login e token | Autenticazione utente (JWT/OAuth) | Flusso login stabile | 3 tentativi falliti bloccano rate | WBS.3.1 | 6/10/14h | 2/3/4g | Alex |
| WBS.3.5.2 | Preferenze notifiche | Modello preferenze e API | Salvataggio e recupero ok | E2E preferenze→invio | WBS.3.5.1 | 4/6/10h | 1/2/3g | Alex |
| WBS.4.3.1 | UI filtri | Filtri categoria/prezzo/orari | Filtri funzionanti | Stato vuoto gestito | WBS.3.2 | 8/12/16h | 2/3/4g | Alice |
| WBS.5.1.1 | Form luogo | Form CRUD con validazioni | Creazione luogo | Errori validazione mostrati | WBS.3.2 | 6/10/14h | 1/2/3g | Alice |

### Policy livello di dettaglio
Si scompone fino a task stimabili entro 2–5 giorni di lavoro, con chiari criteri di completamento. Task più grandi sono “epic” e vengono ulteriormente raffinati in fase di planning dello sprint.
