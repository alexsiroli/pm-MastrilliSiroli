# 2203 — Work Breakdown Structure (WBS) — Ziradò

## RBS.1 — Mappa
La mappa orienta gli utenti nella città mostrando i luoghi più rilevanti con le relative schede.

### RBS.1.1 — Schede locali
- WBS.1.1.1 Creazione del modello dati di una scheda locale con: nome, descrizione, tipologia, indirizzo, giorni e orari, servizi offerti, menù, contatti.
- WBS 1.1.2 Raccolta delle informazioni di ogni locale.
- WBS.1.1.3 Sviluppo di un sistema di creazione, modifica e rimozione di un locale. I gestori possono solo modificare e rimuovere i locali, mentre la creazione è un compito esclusivo degli amministratori.
- WBS.1.1.4 Sviluppo di azioni rapide: chiamata al locale, navigazione mappa, condivisione attraverso app terze.

### RBS.1.2 — Geolocalizzazione e posizionamento luoghi
- WBS.1.2.1 Progettazione e sviluppo di una mappa con grafica intuitiva e gesture di navigazione base. 
- WBS.1.2.2 Raccolta coordinate geografiche di ogni locale ricavate dall'indirizzo del locale.
- WBS.1.2.3 Sviluppo di un sistema di caricamento dei locali come punti nella mappa.
- WBS.1.2.4 Controllo che vengano rispettati i principi fondamentali di accessibilità.

### RBS.1.3 — Tipologie/filtri
- WBS.1.3.1 Definizione delle tipologie di un locale: ristorante, pizzeria, sushi, bar, discoteca, sala giochi, cinema e teatro.
- WBS.1.3.2 Sviluppo di un sistema di filtraggio dei locali in base alla tipologia, orari e fasce di prezzo.

## RBS.2 — Eventi
La sezione eventi racchiude le attività specifiche dei locali con relativi dettagli evento.

### RBS.2.1 — Dettaglio evento
- WBS.2.1.1 Creazione del modello dati di un evento con: titolo, descrizione, location, giorno ed ora, prezzo e locale promotore.

### RBS.2.2 — Caricamento di eventi da gestori
- WBS.2.2.1 Sviluppo di un sistema per i locali di creazione, modifica e rimozione di un evento.
- WBS.2.2.2 Validazioni e gestione contenuti mancanti nel form di creazione/modifica.
- WBS.2.2.3 Notifica in app dell'esito al gestore.

### RBS.2.2 — Calendario e lista con filtri
- WBS.2.3.1 Progettazione e sviluppo di un calendario con grafica intuitiva e gesture di navigazione base. Gli eventi vengono collocati sul calendario in base al giorno in cui si verificano.
- WBS.2.3.2 Progettazione e sviluppo di una lista con grafica intuitiva e gesture di navigazione base. Gli eventi vengono collocati sulla lista in base al giorno in cui si verificano.
- WBS.2.3.3 Sviluppo di un sistema di filtraggio degli eventi in base alla tipologia di locale, giorno, orari e fasce di prezzo.

## RBS.3 — Coupon/Offerte (R2)
Possibilità di visualizzare e aggiungere dei coupon. Il coupon è caratterizzato da una descrizione testuale e da un numero di utilizzi.

### RBS.3.1 — Creazione/gestione coupon da parte dei gestori
- WBS.3.1.1 Creazione del modello dati di un coupon con: titolo, descrizione, limiti, validità e locale promotore.
- WBS.3.1.2 Sviluppo di un sistema per i locali di creazione, modifica e rimozione di un coupon.
- WBS.3.1.3 Notifica in app dell'esito al gestore.

### RBS.3.2 — Utilizzo del coupon da parte dei clienti
- WBS.3.2.1 Sviluppo dell'interfaccia per i clienti per visualizzare i coupon.
- WBS.3.2.2 Sviluppo di un sistema per utilizzare i coupon. Si prevede che vengano consumati in presenza del personale del locale.

## RBS.4 — Recensioni (R3)
Possiblità da parte dei clienti di recensire un locale. Ogni utente può segnalare le recensioni.

### RBS.4.1 — Valutazioni per tipologia di locale
- WBS.4.1.1 Progettazione di un insieme di punti da valutare in base alla tipologia di locale.
- WBS.4.1.2 Sviluppo di un sistema per permettere ai clienti di valutare un locale, secondo i punti relativi alla tipologia. 
- WBS.4.1.3 Analisi base dei punteggi per locale, con possibilità di mostrare la media e l'andamento nel tempo dei punti.
- WBS.4.1.4 Sviluppo dell'interfaccia per visualizzare le valutazioni a punti.

### RBS.4.2 — Recensioni testuali
- WBS.4.2.1 Creazione del modello dati di una recensione con: utente, titolo e descrizione.
- WBS.4.2.2 Sviluppo dell'interfaccia per recensire un locale con validazione della lunghezza dei testi.
- WBS.4.2.3 Sviluppo dell'interfaccia per visualizzare le recensioni testuali.

### RBS.4.3 — Moderazione base
- WBS.4.3.1 Sviluppo dell'interfaccia per segnalare delle recensioni inappropriate da parte di clienti e locali.
- WBS.4.3.2 Sviluppo dell'interfaccia per visualizzare e gestire le segnalazioni per gli amministratori.
- WBS.4.3.3 Notifica al segnalatore dell'esito della moderazione.

## RBS.5 — Backend/API e Admin
L'infrastruttura deve gestire i dati in maniera corretta e coerente.

### RBS.5.1 — Autorizzazione in base al ruolo
- WBS.5.1.1 Login e registrazione tramite email/password o Account Google.
- WBS.5.1.2 Gestione dell'interfaccia coerente al ruolo dell'utente.
 
### RBS.5.2 — Interfaccia per amministratore
- WBS.5.2.1 Creazione del portale admin che permette di eseguire operazioni ordinarie da parte del team, quali creazione/modifica/rimozione di un locale e moderazione delle recensioni.

## RBS.6 — Sistema di Notifiche
Possibilità di ricevere notifiche.

### RBS.6.1 — Notifiche
- WBS.6.1.1 Sviluppo di un sistema che manda notifiche agli utenti. 
- WBS.6.1.2 Trigger per i clienti quando viene inserito/modificato un locale o aggiunte di nuovi coupon ed eventi.
- WBS.6.1.3 Interfaccia che permette agli utenti di selezionare le notifiche che vogliono ricevere.
- WBS.6.1.4 Trigger automatici per i locali per notificare l'esito di un caricamento di evento o coupon e per gli utenti che segnalano recensioni.

## RBS.7 — Requisiti Non Funzionali
Linee guida trasversali per performance, stabilità, rispetto della privacy e di normative e accessibilità base.

### RBS.7.1 — Performance
- WBS.7.1.1 Le viste principali devono caricarsi entro 2 secondi nel 95% dei casi.

### RBS.7.2 — Stabilità
- WBS.7.2.1 Il tasso di crash per sessione resta sotto l’1%.

### RBS.7.3 — Privacy/GDPR (consensi, policy)
- WBS.7.3.1 I processi raccolgono consensi espliciti e mostrano policy trasparenti in linea con GDPR.

### RBS.7.4 — Rispetto delle normative degli store
- WBS.7.4.1 Adesione ai principi richiesti da App Store e Google Play Store.

### RBS.7.5 — Accessibilità base
- WBS.7.5.1 Interfacce e testi rispettano requisiti minimi di accessibilità per un uso inclusivo.
