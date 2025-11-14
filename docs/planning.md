---
layout: page
title: Planning – Ziradò
permalink: /planning/
---
Dopo lo **Scoping**, il team ha obiettivi e funzionalità chiari. Per procedere con **design** e **implementazione** è stata avviata la **pianificazione** al fine di definire le attività da svolgere, stimarne i costi e produrre una schedula che permetta di monitorare l’avanzamento del progetto.

Vengono indette delle riunioni che coinvolgono Alex e Alice.

## **I, II e III sessione**

**Scopo:** individuare le attività da svolgere per il raggiungimento dei requisiti e stimare la durata di ciascuna.

**Esito:** è stata prodotta una **WBS** come estensione della RBS, di seguito riportata:

📂 **Allegato 4 – [4-wbs.md – Work Breakdown Structure (WBS)]({{ '/attachments/4-wbs/' | relative_url }})**

Per stimare le attività di Ziradò è stato adottato un approccio **consensus-based** basato sulla tecnica **Three-Point**. Per ogni task il team ha discusso e annotato tre valori: **Ottimistico (O)**, **Più probabile (M)** e **Pessimistico (P)**. La stima operativa dell’effort è stata calcolata con la **media ponderata**
**E = (O + 4M + P) / 6**, che fornisce una stima più accurata dei tempi.

Poiché siamo studenti e l’impegno settimanale reale oscilla in base a lezioni ed esami, abbiamo fissato assunzioni realistiche di capacità: **20 h/settimana/persona** e **efficienza 75%**, che equivalgono a **15 h/settimana** di lavoro effettivo. Considerando di lavorare dal lunedì al venerdì, si stima che le ore utili siano 3 in un giorno, mentre le effettive siano 4. Nel calcolare il numero di giorni necessario a svolgere una attività (il quale impegno è sempre calcolato in ore), l'operazione _giorni = ore / 3_ queste sono arrotondati per eccesso così da evitare stime troppo ottimistiche.

La stima della durata delle attività è riportata nel seguente file:
📂 **Allegato 5 – [5-stime-e-fabbisogno.md – Stime e Fabbisogno Risorse]({{ '/attachments/5-stime-e-fabbisogno/' | relative_url }})**


La **distribuzione del lavoro** è stata impostata in modo **equilibrato** tra **backend/API e infrastruttura (Alice)** e **frontend/UI (Alex)**. Avendo entrambi svolto lo stesso corso di studio, si suppone che entrambi abbiano lo stesso background: la ripartizione è guidata soprattutto da interesse e continuità sui moduli, non da differenze di skill.


---

## **IV sessione**

**Scopo:** definire la **schedula** del progetto.

**Esito**: partendo dall'analisi delle stime è stato prodotto uno schedula che costruisce un calendario basandosi sulle dipendenze tra le diverse attività e sui periodi di festività. 
Vincoli: 
- Giorni lavorativi: lun–ven; 
- Periodi di festività: 24/12→07/01 e dal 01/04→08/04.
- Giorno di inizio progetto: 01/12/2025

Di seguito è riportato il **Gantt** costruito:

📂 **Allegato 7 – [7-gantt.md – Schedula Gantt]({{ '/attachments/7-gantt/' | relative_url }})**

Dato lo schedula, si procede con il caricamento delle singole attività all'interno del software Trello che, adottando una metodologia SCRUM, permette di tenere traccia dello stato di avanzamento delle singole attività.
È stata prevista una **scope bank** pari al **10%** del tempo totale di progetto per assorbire ritardi e imprevisti.


---

## **V sessione**

**Scopo:** identificare i **rischi** del progetto e i relativi piani.
**Esito:** è stato compilato un documento di analisi dei rischi, fondamentale per avere chiaro ciò che potrebbe ostacolare il completamento del progetto.

📂 **Allegato 8 – [8-risk-analysis.md – Analisi Rischi e Mitigazione]({{ '/attachments/8-risk-analysis/' | relative_url }})**

## **VI sessione**

**Scopo:** effettuare un'analisi relativa ai costi diretti e indiretti per lo sviluppo.
**Esito:**è stato compilato il seguente documento:

📂 **Allegato 6 – [6-analisi-costi.md – Analisi Costi e Budget]({{ '/attachments/6-analisi-costi/' | relative_url }})**

## **VII sessione**
**Scopo:** produrre il Project Definition Statement.

📂 **Allegato 3 – [3-pds.md – Project Definition Statement (PDS)]({{ '/attachments/3-pds.md' | relative_url }})**
