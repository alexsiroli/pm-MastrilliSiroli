---
layout: page
title: Scoping – Ziradò
permalink: /scoping/
---
## **Contesto**

Ziradò è un'applicazione pensata per mappare locali ed eventi offerti nella città di Cesena, con l’obiettivo di favorire turismo locale e coinvolgimento dei cittadini.
**Non esiste un committente unico**: l'idea è sviluppare da zero un'idea innovativa che poi possa essere effettivamente utilizzata dai gestori di Cesena. Pertanto, i membri del team collaborano attivamente per cercare di capire e individuare al meglio tutti i possibili bisogni e desideri dell’utenza finale del prodotto.

Per definire le caratteristiche e le funzionalità del progetto vengono indette delle specifiche riunioni.

---

## **Riunione di definizione del progetto (scoping meeting)**

**Scopo:** individuazione delle aspettative e dei requisiti dell’applicazione.

### **Partecipanti della riunione**

| **Membro**                                     | **Ruolo**                       |
| ---------------------------------------------- | ------------------------------- |
| **Alex Siroli**                                | Project Manager |
| **Alice Mastrilli**                                      | Core Team Member  |

### **Agenda**

* **Introduzione** (a cura del PM)
* **Scopo della riunione** (a cura del PM)
* **Descrizione del contesto di Ziradò**
* **Descrizione degli indicatori di successo**
* **Descrizione dei deliverable del progetto**
* **Definizione dei requisiti**
* **Scelta del modello PMLC da seguire**
* **Bozza e approvazione del POS**

### **Sintesi svolgimento**

Dagli incontri è emerso che: 
## Contesto e Assunzioni
- Target: cittadini e turisti di Cesena; esercenti e associazioni locali.
- Vincoli: ambito territoriale iniziale, tempo limitato dell’elaborato, budget minimo, policy store (Apple/Google), GDPR.
- Assunzioni: disponibilità di contenuti dai locali, sponsorship iniziale da entità locali, mappe con free tier sufficiente, hosting low‑cost.
- Tecnologie (ipotesi): mobile cross‑platform.

Per la definizione dei requisiti sono stati necessari diversi incontri per mettere a punto le principali funzionalità dell'applicativo. Per avere un'idea ancora più pratica di ciò in cui i locali riscontrano meno pubblico, sono stati intervistati dei gestori di tre diverse tipologie di attività: una sala giochi, un ristorante e una gelateria.
Tali gestori resteranno un punto di riferimento nel corso dello sviluppo, per risolvere eventuali dubbi che possono sorgere nelle fasi successive.
L'insieme dei requisiti sono stati definiti nel seguente documento:

📂 **Allegato 2 – [2-rbs.md – Requirements Breakdown Structure (RBS)]({{ '/attachments/2-rbs/' | relative_url }})**

Una sintesi delle riunioni, con considerazioni su obbiettivi, criteri di successo e rischi è disponibile in:

📂 **Allegato 1 – [1-pos.md – Project Overview Statement (POS)]({{ '/attachments/1-pos/' | relative_url }})**


## **Scelta del modello PMLC**
Si è scelto di adottare un modello PMLC **ibrido iterativo-incrementale** con sprint time-boxed e milestone fisse perché permette di mantenere una struttura chiara pur lasciando la flessibilità necessaria ad adattarsi ai feedback e alle incertezze del progetto. Nel nostro caso non puntiamo a rilasci continui, ma a **tre release principali**, ciascuna dedicata all’introduzione di nuove funzionalità significative. Questo approccio è particolarmente adatto perché i requisiti core sono già noti, mentre rimangono elementi da validare legati all’esperienza d’uso e ai contenuti. Essendo il team composto da sole due persone, il modello ibrido consente di lavorare in modo ordinato, senza l’eccessiva rigidità dei modelli lineari ma nemmeno con la frammentazione tipica degli approcci a rilasci molto frequenti. In questo modo possiamo procedere per passi, mantenere il controllo delle milestone e introdurre nuove funzioni in maniera progressiva e sostenibile.
