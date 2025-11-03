# RBS - Ziradò  
**(Requirements Breakdown Structure)**  

---

## **1. Realizzazione dell'app**

### 1.1 Mockup e design system
- **Output atteso:** prototipi ad alta fedeltà per i flussi utente ed esercente e un design system condiviso (palette, tipografia, componenti).
- **Criteri di accettazione:**
  - Copertura del 100% dei flussi principali (onboarding, mappa, lista eventi, lista locali, dettaglio locale, gestione eventi/coupon, dashboard esercente).
  - Approvazione formale del committente registrata a verbale.
  - Linee guida di stile archiviate nel repository design e conformi a WCAG 2.1 AA.

### 1.2 Funzionalità lato utente
- **Output atteso:** moduli applicativi per mappa interattiva, calendario eventi e catalogo locali integrati con i dati aggiornati.
- **Criteri di accettazione:**
  - *Completezza:* filtri per data, categoria, distanza e disponibilità di coupon abilitati su tutte le viste.
  - *Performance:* tempo di caricamento iniziale delle viste principali ≤ 2 s (95° percentile) su rete 4G con dataset di test ≥ 200 locali.
  - *Reliability:* tasso di errore delle chiamate API critiche < 1% su finestra mobile di 7 giorni con alert automatici.
  - *Testability:* suite end-to-end che copre almeno il 90% dei percorsi critici (ricerca evento, apertura scheda locale, salvataggio preferiti).
  - *Look and Feel:* interfaccia conforme al design system approvato senza deviazioni non documentate.

### 1.3 Funzionalità lato esercente
- **Output atteso:** pannello esercente per gestione informazioni attività, eventi, coupon e statistiche d'uso.
- **Criteri di accettazione:**
  - *Completezza:* sezioni per dati anagrafici, calendario eventi, gestione coupon e pannello analitiche disponibili al rilascio.
  - *Validity:* feedback raccolto da almeno 3 esercenti pilota prima dell'approvazione finale.
  - *Maintainability:* componenti UI riutilizzabili documentati nel design system e guideline di sviluppo aggiornate.
  - *Measurability:* ogni coupon/evento deve esporre metriche di conversione e visualizzazioni aggiornate giornalmente.
  - *Safety:* permessi di modifica granulari con tracciamento audit di ogni variazione.

### 1.4 Gestione account esercenti e sicurezza
- **Output atteso:** processo di onboarding esercenti, gestione ruoli e misure di sicurezza applicativa.
- **Criteri di accettazione:**
  - *Safety:* autenticazione a due fattori opzionale, policy password (min 10 caratteri, complessità) e cifratura dati sensibili in transito e a riposo.
  - *Reliability:* disponibilità servizi di autenticazione ≥ 99% su base mensile con monitoraggio in tempo reale.
  - *Stabilità:* gestione delle richieste di cambio dati tramite workflow approvativo e logging completo.
  - *Specifications:* manuale operativo per l'onboarding pubblicato e versionato con numero di revisione.

### 1.5 Testing automatizzato e con utenti
- **Output atteso:** piano di test, suite automatizzata e sessioni di validazione con utenti reali.
- **Criteri di accettazione:**
  - Copertura di test unitari ≥ 80% sui moduli core (mappa, eventi, gestione coupon).
  - Almeno 2 cicli di test di usabilità con 10 utenti finali e report delle evidenze con priorità di risoluzione.
  - Piano di regressione automatica eseguito a ogni release con storico risultati accessibile al team.

---

## **2. Preparazione dei contenuti**

### 2.1 Raccolta iniziale dati locali
- **Output atteso:** dataset strutturato dei locali del centro di Cesena con immagini e metadati.
- **Criteri di accettazione:**
  - Copertura minima del 75% dei locali identificati nel perimetro "centro" validata da camera di commercio o associazioni categoria.
  - Per ogni locale: foto autorizzata, geolocalizzazione, fascia di prezzo, orari, giorni di apertura e contatti verificati.
  - Evidenza della validazione dati firmata dal responsabile contenuti.

### 2.2 Qualità e standardizzazione dei dati
- **Output atteso:** linee guida di data quality e procedure di arricchimento/normalizzazione.
- **Criteri di accettazione:**
  - *Measurability:* ≥ 98% dei record con tutti i campi obbligatori valorizzati; tolleranza massima errori ortografici 1% tramite campionamento.
  - *Maintainability:* dizionario dati e template di importazione pubblicati in repository condiviso.
  - *Testability:* script di validazione automatica eseguiti ad ogni import con log degli esiti.

### 2.3 Caricamento e aggiornamento contenuti
- **Output atteso:** pipeline di caricamento nel CMS/app e processo di aggiornamento continuo.
- **Criteri di accettazione:**
  - Tempo medio di pubblicazione nuovi contenuti ≤ 2 giorni lavorativi dal completamento raccolta.
  - Revisione periodica mensile con report su variazioni (nuove aperture, chiusure, cambi orari).
  - Backup completo del dataset dei contenuti eseguito giornalmente e conservato per 30 giorni.

---

## **3. Ricerca degli sponsor**

### 3.1 Mappatura e contatto sponsor target
- **Output atteso:** elenco qualificato di potenziali sponsor e piano di contatto.
- **Criteri di accettazione:**
  - Almeno 15 potenziali sponsor profilati per settore e budget stimato.
  - Script di contatto e materiali di presentazione approvati dal committente.
  - CRM o foglio di tracciamento aggiornato settimanalmente con stato di avanzamento.

### 3.2 Offerte commerciali e contratti
- **Output atteso:** pacchetti di sponsorizzazione, business case e processi di firma.
- **Criteri di accettazione:**
  - Tre livelli di pacchetto (bronze, silver, gold) con benefici, costi, KPI promessi e SLA di erogazione.
  - Template contrattuale revisionato dall'ufficio legale e versionato.
  - *Validity:* approvazione del committente su pricing e condizioni prima dell'invio agli sponsor.

### 3.3 Integrazione banner e tracciamento
- **Output atteso:** funzionalità per la visualizzazione dinamica dei banner sponsor nell'app e reportistica correlata.
- **Criteri di accettazione:**
  - *Performance:* impatto sulla latenza di caricamento schermate ≤ 200 ms nel 95° percentile.
  - *Reliability:* disponibilità del servizio di ad serving ≥ 99% e fallback in caso di errore.
  - *Testability:* tracciamento click/impression integrato con dashboard e dati esportabili mensilmente.
  - *Safety:* conformità GDPR con gestione consensi e anonimizzazione analytics.

---

## **4. Lancio e marketing**

### 4.1 Identità visiva e storytelling
- **Output atteso:** logo, linee guida brand, kit grafico e storytelling di progetto.
- **Criteri di accettazione:**
  - Manuale brand con palette, tipografia, uso logo e tone of voice pubblicato in repository condiviso.
  - Tre concept di storytelling testati con focus group interno e scelto quello approvato dal committente.
  - Materiali grafici consegnati in formati ottimizzati (SVG, PNG, PDF) e verificati per coerenza.

### 4.2 Pubblicazione sugli store
- **Output atteso:** app disponibile su Google Play e App Store con schede descrittive ottimizzate.
- **Criteri di accettazione:**
  - Checklist di conformità store (privacy, policy contenuti, asset grafici) completata e archiviata.
  - Test di installazione su almeno 5 device Android e 5 device iOS rappresentativi.
  - Analytics configurati (installazioni, retention, crash) prima del go-live.

### 4.3 Campagne di attivazione
- **Output atteso:** piano di campagne rivolte a utenti e esercenti con budget e calendario.
- **Criteri di accettazione:**
  - Mix di canali (social, manifesti, QR code, email) con KPI target definiti (acquisizione, conversione, CAC).
  - Budget allocato e approvato, con monitoraggio settimanale delle performance.
  - Contenuti social pianificati almeno 4 settimane prima del lancio con copy approvati.

### 4.4 Formazione esercenti e supporto
- **Output atteso:** materiale formativo, sessioni di onboarding e piano di supporto post-lancio.
- **Criteri di accettazione:**
  - Manuale operativo e video tutorial disponibili per gli esercenti entro la data di lancio.
  - Almeno 2 sessioni formative (in presenza o webinar) con registrazione presenze e feedback.
  - Canale di supporto dedicato attivo (email o chat) con SLA di risposta ≤ 1 giorno lavorativo.

---

## **5. Monitoraggio e manutenzione**

### 5.1 Monitoraggio soddisfazione e utilizzo
- **Output atteso:** sistema di raccolta feedback e indicatori di soddisfazione.
- **Criteri di accettazione:**
  - Sondaggi trimestrali per utenti ed esercenti con target di risposta ≥ 20% e NPS minimo di 30.
  - Dashboard mensile con metriche di utilizzo (MAU, retention, coupon redemption) disponibile al management.
  - Piano di azioni correttive entro 10 giorni lavorativi per ogni criticità ad alta priorità.

### 5.2 Aggiornamento catalogo e nuovi locali
- **Output atteso:** processo continuo di onboarding nuovi locali e revisione schede esistenti.
- **Criteri di accettazione:**
  - Inserimento di nuovi locali entro 5 giorni lavorativi dalla richiesta e audit semestrale di tutto il catalogo.
  - Verifica documentata delle variazioni di orari/prezzi almeno ogni trimestre.
  - Registro delle richieste di aggiornamento con stato e data di completamento.

### 5.3 Manutenzione tecnica e prestazioni
- **Output atteso:** roadmap di release, monitoraggio prestazioni e piano di continuità operativa.
- **Criteri di accettazione:**
  - Ciclo di release regolare (almeno una minor release ogni 6 settimane) con changelog pubblicato.
  - Monitoraggio prestazioni h24 con soglie di alert definite; MTTR (Mean Time To Restore) target ≤ 4 ore per incidenti critici.
  - Documentazione tecnica aggiornata a ogni release (architettura, API, manuale gestione infrastruttura).

### 5.4 Gestione cambi requisiti e governance
- **Output atteso:** processo strutturato di change management e allineamento stakeholder.
- **Criteri di accettazione:**
  - Comitato di revisione requisiti riunito almeno mensilmente con verbali archiviati.
  - Valutazione di impatto (costo, tempo, rischio) obbligatoria per ogni change request prima dell'approvazione.
  - Registro versioni RBS/WBS aggiornato, con tracciabilità delle modifiche e notifica al team entro 2 giorni lavorativi.
