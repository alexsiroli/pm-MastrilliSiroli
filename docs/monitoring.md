---
layout: page
title: Monitoring & Controlling – Ziradò
permalink: /monitoring/
---
## Sistema di reporting (Ziradò)

Per Ziradò adottiamo un approccio **SCRUM appoggiato al Gantt**: il Gantt resta la nostra bussola temporale con milestone e dipendenze; **Trello** è lo strumento operativo con cui seguiamo lo sviluppo giorno per giorno. 

Tutto ciò che appare nello schedula (il Gantt) va caricato in Trello: una card per ogni step del piano. Ogni card contiene:

* **descrizione chiara del task** (cosa deve succedere per dire “finito”),
* **date** coerenti con il Gantt (inizio/fine),
* **chi se ne occupa** (Alex o Alice).

In questo modo possiamo **verificare se il piano viene rispettato** guardando l’avanzamento reale in Trello; se qualcosa slitta ci se ne accorge immediatamente.

La board Trello usa cinque colonne:
Backlog → Da Fare → In esecuzione → Problemi → Fatto.
Il flusso “naturale” è Backlog → Da Fare → In esecuzione → Fatto. La colonna "Problemi" non è uno step obbligatorio: è un parcheggio temporaneo per le card che hanno un dubbio reale o un ostacolo. Serve a non perdere di vista i blocchi: quando spostiamo una card in Problemi, annotiamo *brevemente* che cosa ci frena e rimandiamo ai dettagli (vedi sotto i file dei problemi). Appena il dubbio è chiarito, la card torna in "In esecuzione".

Lo sprint dura **1 settimana**; ogni lunedì e venerdì facciamo un allineamento breve. Durante l'incontro, ciascuno mostra cosa ha implementato, se serve si fa un po’ di brainstorming, si verifica cosa è rimasto indietro rispetto al Gantt, e si fissano i micro-obiettivi per i giorni successivi.

Anche se con Trello è possibile visualizzare in maniera semplice lo stato di esecuzione del progetto, ogni venerdì, per avere anche un indicatore numerico, si calcola lo **Schedule Performance Index (SPI)**:

### **SPI = EV / PV**

- EV (Earned Value): “valore guadagnato”, cioè il lavoro davvero completato fino a oggi, espresso nelle stesse unità della pianificazione (per Ziradò: ore stimate o giorni effettivi da 3h).

- PV (Planned Value): “valore pianificato”, cioè il lavoro che avremmo dovuto completare entro oggi secondo la baseline (Gantt/sprint).

**Interpretazione rapida**

- SPI = 1,00 → in linea con il piano.

- SPI > 1,00 → in anticipo (abbiamo completato più di quanto previsto).

- SPI < 1,00 → in ritardo (abbiamo completato meno del previsto).




## Issues Log

Per i **problemi** adottiamo una doppia traccia:

1. **Segnale veloce in Trello**:
   se un task ha un intoppo, **spostiamo la card in “Problemi”** e scriviamo due righe di nota (“che cosa blocca e da quando”). Questo ci dà **visibilità immediata**: è chiaro a colpo d’occhio cosa non sta scorrendo.

2. **Approfondimento nei file personali**:
   i dettagli li conserviamo in due file di testo, **problemiAlice.md** e **problemiAlex.md**: qui scriviamo note più dettagliate sul problema riscontrato: contesto, tentativi fatti, link utili, ipotesi di fix. 
   
   Quando decidiamo insieme cosa fare, la card esce da **Problemi** e rientra in **In esecuzione**. Il problema viene eliminato dal file problemi*Nome*.md e la soluzione adottata viene messa nel file `DECISION.md`

---


