---
layout: page
title: 3-pds.md – Project Definition Statement (PDS)
permalink: /attachments/3-pds/
---

# **Project Definition Statement (PDS) – Ziradò**

## 1) Scopo e motivazione

Realizzare un’app **mobile** che unifichi **mappa dei locali e relative informazioni**, **bacheca eventi**, **coupon specifici per locale** e **sistema di recensioni** per Cesena, incrementando partecipazione e ricavi degli operatori locali.

**Motivazione:** mancanza di un canale unico affidabile e aggiornato.

## 2) Obiettivi misurabili

* **R1** attiva **entro 31/07/2026**, **R2** entro i 3 mesi successivi al lancio di R1, **R3** entro i 3 mesi successivi a R2.
* **Qualità:** Il tempo di caricamento del 95% delle schermate principali è inferiore a 2 secondi e il tasso di crash per sessione è inferiore all’1%.
* **Adozione:** 5.000 download e rating ≥ 4.0 entro 12 mesi in entrambi gli store di lancio.
* **Ecosistema esercenti:** 75% locali centro storico a 12 mesi.
* **Economia:** break-even di cassa entro 6 mesi dal lancio.

## 3) Deliverable

* **R1:** Mappa + schede locali, eventi (CRUD, calendario/lista/filtri), login/ruoli, admin, notifiche base, publishing store, requisiti non funzionali.
* **R2:** **Coupon/offerte** e notifiche dedicate.
* **R3:** **Recensioni** (tramite voti o descrizione testuale) con **moderazione** e notifiche correlate.

## 4) Vincoli

* **Tempo:** rispetto del calendario Gantt ([7-gantt.md – Schedula Gantt e Network Diagram]({{ '/attachments/7-gantt/' | relative_url }})), con periodi **24/12/2025–07/01/2026** e **01/04/2026–08/04/2026** esclusi.
* **Team:** 2 persone, **15 h/sett** ciascuno.
* **Budget diretto:** circa **404 €**/primo anno + pubblicità di lancio (dettagli in [6-analisi-costi.md – Analisi Costi e Budget]({{ '/attachments/6-analisi-costi/' | relative_url }})).
* **Store policy/GDPR** obbligatorie per la pubblicazione.

## 5) Assunzioni chiave

* Collaborazione degli **esercenti** per la fornitura e l’aggiornamento dei contenuti.
* Quote **Firebase** e **Mappe** adeguate ai volumi di utenti e dati previsti.
* **Supporto istituzionale minimo** (Comune) per la promozione e la visibilità del progetto.
* **Compatibilità cross-platform** stabile (iOS/Android) garantita dai framework scelti.
* Accesso continuativo agli strumenti di sviluppo (**Firebase, GitHub, IDE, API mappe**) senza interruzioni o modifiche di licenza.
* Permanenza dei membri del team: **Alex e Alice** restano attivamente coinvolti per l’intera durata del progetto.

## 6) Stakeholder e governance

| **Ruolo**                               | **Nome** | **Responsabilità**                   |
| --------------------------------------- | -------- | ------------------------------------ |
| **PM / Responsabile Frontend**          | **Alex** | Piano, scope, UX, store, sponsor     |
| **Tech Lead / Responsabile Backend**    | **Alice**| Architettura, sicurezza, API, build  |
| **Esercenti pilota**                    | –        | Dati locali, eventi, coupon          |
| **Sponsor/Comune**                      | Cesena   | Co-marketing, visibilità             |
| **Utenti pilota**                       | –        | Feedback, rating store               |

**RACI sintetico**

| **Attività**                             | **R** | **A** | **C**     | **I**      |
| ---------------------------------------- | ----- | ----- | --------- | ---------- |
| Pianificazione e obiettivi del progetto  | Alex  | Alex  | Alice     | Sponsor    |
| Struttura tecnica e sicurezza            | Alice | Alice | Alex      | –          |
| Grafica, interfaccia e contenuti         | Alex  | Alex  | Esercenti | Sponsor    |
| Pubblicazione sugli store                | Alex  | Alex  | Alice     | Sponsor    |
| Comunicazione e social media             | Alex  | Alex  | Sponsor   | Esercenti  |
| Regole sulla privacy e GDPR              | Alice | Alex  | –         | Sponsor    |

*(A=Approva – R=Responsabile – C=Consultato – I=Informato)*

## 7) Piano temporale e milestone

| **Milestone**               | **Data**       |
| --------------------------- | -------------- |
| Start R1                    | 01/12/2025     |
| Feature complete R1         | 20/06/2026     |
| Go-Live R1 (store approved) | **31/07/2026** |
| Start R2                    | 01/08/2026     |
| Go-Live R2                  | 16/09/2026     |
| Start R3                    | 15/10/2026     |
| Go-Live R3                  | 30/11/2026     |
