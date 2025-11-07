# 2102 — Requirements Breakdown Structure (RBS) — Ziradò

## Struttura
| Numero | Titolo | Descrizione | Misurabilità |
| --- | --- | --- | --- |
| RBS.1 | **Mappa** | La mappa orienta gli utenti nella città mostrando i luoghi più rilevanti con le relative schede locali. | La mappa contiene il 75% dei locali d'interesse per l'app. |
| RBS.1.1 | **Schede locali** | Le schede sintetizzano orari, servizi disponibili, eventuali menù e contatti per facilitare la scelta del locale. | 
| RBS.1.2 | **Geolocalizzazione e posizionamento luoghi** | Ogni locale è geolocalizzato con coordinate geografiche affidabili e aggiornate. | Accuratezza media inferiore a 50 metri. |
| RBS.1.3 | **Tipologie/filtri** | Tipologie e filtri permettono di selezionare i luoghi per tipologia, fascia di prezzo e giorni/orari di apertura. Nella prima release si prevede di inserire le tipologie: ristorante, pizzeria, sushi, bar, discoteca, sala giochi, cinema e teatro.  | Le tipologie devono rappresentare il 100% dei locali. |
| RBS.2 | **Eventi** | La sezione eventi racchiude le attività specifiche dei locali con relativi dettagli evento. |
| RBS.2.1 | **Dettaglio evento** | La scheda evento racchiude descrizione, location, fascia oraria e prezzo.
| RBS.2.2 | **Caricamento di eventi da gestori** | Gestori di locali possono proporre nuovi eventi che vengono pubblicati automaticamente. | L'evento deve essere visualizzabile entro 5 minuti dalla creazione. |
| RBS.2.3 | **Calendario e lista con filtri** | Un calendario filtrabile per data e tipologia di locali consente di individuare più velocemente gli eventi d'interesse all'utente. |
| RBS.3 | **Coupon/Offerte (R2)** | Possibilità di visualizzare e aggiungere dei coupon. Il coupon è caratterizzato da una descrizione testuale e da un numero di utilizzi.  |
| RBS.3.1 | **Creazione/gestione coupon da parte dei gestori** | I gestori dei locali possono configurare e creare i coupon in autonomia, adattandoli alle proprie esigenze. | Il coupon deve essere visualizzato entro 5 min dalla propria creazione. |
| RBS.3.2 | **Utilizzo del coupon da parte dei clienti** | I clienti possono utillzzare i coupon in base alle specifiche dettate dal gestore. | Ogni cliente può utilizzare il coupon il numero massimo di volte specificato dal gestore.|
| RBS.4 | **Recensioni (R3)** | Possiblità da parte dei clienti di recensire un locale. Ogni utente può segnalare le recensioni. |  |
| RBS.4.1 | **Valutazioni per tipologia di locale** | In base alla tipologia di locale, l'utente è invitato a esprimere una votazione numerica nelle diverse domande a lui proposte. | Per ogni tipologia di locale, devono essere presenti almeno 5 diverse specifiche da valutare. |
| RBS.4.2 | **Recensioni testuali** | Gli utenti esprimono libere opinioni relative ad un locale. |  |
| RBS.4.3 | **Moderazione base** | Se viene segnalata una recensione, i gestori dell'applicativo possono confermare o eliminare la recensione segnalata. | |
| RBS.5 | **Backend/API e Admin** | L'infrastruttura deve gestire i dati in maniera corretta e coerente. |  |
| RBS.5.1 | **Autorizzazione in base al ruolo** | L'applicazione richiede il login e fornisce autorizzazioni coerenti con i ruoli. | 100% degli endpoint sensibili richiede autenticazione e log di audit completi. |
| RBS.5.2 | **Interfaccia per amministratore** | Un ambiente gestionale che permette di eseguire operazioni ordinarie da parte del team, quali creazione/modifica/rimozione di un locale e moderazione delle recensioni. |
| RBS.6 | **Sistema di Notifiche** | Possibilità di ricevere notifiche.   |  |
| RBS.6.1 | **Notifiche** | Le notifiche informano gli utenti su eventi o offerte rilevanti. Ogni utente può scegliere il tipo di notifica che vuole ricevere, tra: inserimento/modifica dei locali, aggiunta di nuove offerte o eventi. | Il sistema di notifiche deve funzionare correttamente sia su iOS che Android. Ricezione notifica di test confermata su almeno 5 device. |
| RBS.7 | **Requisiti Non Funzionali** | Linee guida trasversali per performance, stabilità, rispetto della privacy e di normative e accessibilità base. | |
| RBS.7.1 | **Performance** | Le viste principali devono caricarsi entro 2 secondi nel 95% dei casi. |  |
| RBS.7.2 | **Stabilità** | Il tasso di crash per sessione resta sotto l’1%. | |
| RBS.7.3 | **Privacy/GDPR (consensi, policy)** | I processi raccolgono consensi espliciti e mostrano policy trasparenti in linea con GDPR. | |
| RBS.7.4 | **Rispetto delle normative degli store** | Adesione ai principi richiesti da App Store e Google Play Store. | Il 100% delle richieste degli store devono essere soddisfatte, la versione beta supera validazioni automatiche. |
| RBS.7.5 | **Accessibilità base** | Interfacce e testi rispettano requisiti minimi di accessibilità per un uso inclusivo. | Superamento test WCAG 2.1 livello AA sulle principali viste. |
