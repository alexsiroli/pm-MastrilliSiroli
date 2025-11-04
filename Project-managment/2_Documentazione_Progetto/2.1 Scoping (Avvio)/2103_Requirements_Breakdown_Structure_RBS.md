# Requirements Breakdown Structure (RBS) — Ziradò

## Struttura
| Numero | Titolo | Descrizione | Misurabilità |
| --- | --- | --- | --- |
| RBS.1 | **Mappa** | La mappa orienta gli utenti nella città mostrando i luoghi più rilevanti con le relative schede locali. | La mappa contiene il 75% dei locali d'interesse per l'app. |
| RBS.1.1 | **Geolocalizzazione e posizionamento luoghi** | Ogni locale è geolocalizzato con coordinate geografiche affidabili e aggiornate. | Accuratezza media inferiore a 50 metri. |
| RBS.1.2 | **Schede locali** | Le schede sintetizzano orari, servizi disponibili, eventuali menù e contatti per facilitare la scelta del locale. | 
| RBS.1.3 | **Categorie/filtri** | Categorie e filtri permettono di selezionare i luoghi per tipologia, fascia di prezzo e giorni/orari di apertura. Nella prima release si prevede di inserire le tipologie: ristorante, pizzeria, sushi, bar, discoteca, sala giochi, cinema e teatro.  | Le tipologie devono rappresentare il 100% dei locali. |
| RBS.2 | **Eventi** | La sezione eventi racchiude le attività specifiche dei locali con relativi dettagli evento. |
| RBS.2.1 | **Calendario e lista con filtri** | Un calendario filtrabile per data e tipologia di locali consente di individuare più velocemente gli eventi d'interesse all'utente. |
| RBS.2.2 | **Dettaglio evento** | La scheda evento racchiude contenuto, location, fascia oraria e prezzo.
| RBS.2.3 | **Caricamento di eventi da gestori** | Gestori di locali possono proporre nuovi eventi che vengono pubblicati automaticamente. | L'evento deve essere visualizzabile entro 5 minuti dalla creazione. |
| RBS.3 | **Coupon/Offerte (R2)** | I gestori dei locali possono creare dei coupon utilizzabili dai clienti. Il coupon è caratterizzato da una descrizione testuale. |
| RBS.3.1 | **Creazione/gestione coupon da parte dei gestori** | I gestori configurano e programmano i coupon in autonomia, adattandoli alle proprie esigenze. | Ruolo "esercente" abilita creazione/modifica/archiviazione; permessi e vincoli verificati in QA. |
| RBS.3.2 | **Utilizzo del coupon da parte dei clienti** | I clienti possono utillzzare i coupon in base alle specifiche dettate dal gestore. | Ogni redemption genera record univoco con timestamp e origine; coerenza UI↔DB al 100% nei test. |
| RBS.4 | **Recensioni (R3)** | Possiblità da parte dei clienti di recensire un locale. | Sistema recensioni attivo (valutazioni + testo) con moderazione e protezioni anti‑spam operative. |
| RBS.4.1 | **Valutazioni per tipologia di locale** | In base alla tipologia di locale, l'utente è invitato a esprimere una votazione numerica nelle diverse domande a lui proposte. | Campi numerici obbligatori enforced; invio bloccato senza valutazioni richieste. |
| RBS.4.2 | **Recensioni testuali** | Gli utenti esprimono libere opinioni relative ad un locale. | Validazione lunghezza minima (≥30 caratteri) e filtro contenuti inappropriati attivi. |
| RBS.4.3 | **Moderazione base** | Una moderazione essenziale da parte dei gestori dell'applicativo mantiene il tono costruttivo delle recensioni e blocca contenuti inappropriati. | Workflow segnalazioni con stati (aperta/in lavorazione/risolta) e SLA configurato. |
| RBS.5 | **Backend/API e Admin** | L'infrastruttura deve gestire i dati in maniera corretta e coerente. | Auth, autorizzazioni, rate limit e audit log abilitati; test unit/integration verdi su endpoint critici. |
| RBS.5.1 | **Autorizzazione in base al ruolo** | L'applicazione richiede il login e fornisce autorizzazioni coerenti con i ruoli. | 100% degli endpoint sensibili richiede autenticazione e log di audit completi. |
| RBS.5.2 | **Admin portal minimo** | Un ambiente gestionale che permette di eseguire operazioni ordinarie da parte del team, quali creaione/modifica/rimozione di un locale e moderazione delle recensioni. | CRUD locali, gestione utenti base e moderazione disponibili; test E2E pass. |
| RBS.6 | **Sistema di Notifiche** | Canale di comunicazione verso gli utenti per eventi e offerte rilevanti. | Infrastruttura push (APNs/FCM) configurata; opt‑in conforme; invio test riuscito su iOS/Android. |
| RBS.6.1 | **Notifiche** | Le notifiche informano gli utenti su eventi o offerte rilevanti. | Percorso opt‑in/opt‑out funzionante; ricezione notifica di test confermata su 3 device. |
| RBS.7 | **Requisiti Non Funzionali** | Linee guida trasversali per performance, qualità e compliance del prodotto. | Monitoraggio attivo per tutti gli indicatori con dashboard e alert configurati. |
| RBS.7.1 | **Performance** | Le viste principali devono caricarsi entro 2 secondi nel 95% dei casi. | P95 tempo di caricamento monitorato con alert automatici. |
| RBS.7.2 | **Stabilità** | Il tasso di crash per sessione resta sotto l’1%. | Crash-free sessions ≥99% su base mensile. |
| RBS.7.3 | **Privacy/GDPR (consensi, policy)** | I processi raccolgono consensi espliciti e mostrano policy trasparenti in linea con GDPR. | 100% degli utenti ha tracciamento del consenso e audit privacy trimestrale senza non conformità. |
| RBS.7.4 | **Rispetto delle normative degli store** | Adesione ai principi richiesti da App Store e Google Play Store. | Checklist store compliance completata; build pre‑submission supera validazioni automatiche. |
| RBS.7.5 | **Accessibilità base** | Interfacce e testi rispettano requisiti minimi di accessibilità per un uso inclusivo. | Superamento test WCAG 2.1 livello AA sulle principali viste. |
