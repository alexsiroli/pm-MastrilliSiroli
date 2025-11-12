# **Scoping — Ziradò**

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
| **Alex Siroli**                                | Product Owner & Project Manager |
| **Alice**                                      | Core Team Member  |

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
## 1) Contesto e Assunzioni
- Target: cittadini e turisti di Cesena; esercenti e associazioni locali.
- Vincoli: ambito territoriale iniziale, tempo limitato dell’elaborato, budget minimo, policy store (Apple/Google), GDPR.
- Assunzioni: disponibilità di contenuti dai locali, sponsorship iniziale da entità locali, mappe con free tier sufficiente, hosting low‑cost.
- Tecnologie (ipotesi): mobile cross‑platform, backend REST, DB cloud, mappe (OpenStreetMap/Mapbox), analytics.

## 2) Indicatori di Successo e Metriche
- IRACIS: Increase Revenue (incremento spesa locale via coupon), Avoid Cost (riduzione dispersione info per i cittadini), Improve Service (unico punto di accesso eventi/attività/luoghi).
- KPI: MAU ≥ 500 (M2), ≥ 1.500 (M3); ≥ 50 eventi attivi/mese (M2); ≥ 30 esercenti registrati (M3); Retention D30 ≥ 20%; Rating store ≥ 4.0; Conversione coupon ≥ 5% utenti attivi; Sponsorship ≥ 2 entro M3.
- Soglie e early warning: SPI/CPI < 0,9 → azione correttiva; MAU < 60% target → sprint dedicato a growth/UX.

Per la definizione dei requisiti sono stati necessari diversi incontri per mettere a punto le principali funzionalità dell'applicativo. Per avere un'idea ancora più pratica di ciò in cui i locali riscontrano meno pubblico, sono stati intervistati dei gestori di tre diverse tipologie di attività: una sala giochi, un ristorante e una gelateria.

L'insieme dei requisiti sono stati definiti nel seguente documento:
📂 **Allegato** **RBS**, **Allegato 1**.

Una sintesi delle riunioni, con considerazioni su obbiettivi, criteri di successo e rischi è disponibile in:

📂 **Allegato** **POS**, **Allegato 2**.


## **Scelta del modello PMLC**
Si è ritenuto che il miglior modello PMLC è quello Ibrido Iterativo‑Incrementale, con timebox a sprint e milestone fisse (pilot locale → estendibile).
- Ragioni della scelta: requisiti core noti ma forte incertezza su adozione, contenuti e UX; team ridotto (2 persone); necessità di rilasci progressivi per testare valore e raccogliere feedback.
- Implicazioni operative: pianificazione iniziale del MVP e milestone, backlog dinamico, change control leggero, misurazione continua dei KPI d’adozione.
