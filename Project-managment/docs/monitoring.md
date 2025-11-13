# **Monitoring & Controlling — Ziradò**

# Sistema di reporting (Ziradò)

Per Ziradò adottiamo un approccio **SCRUM “light” appoggiato al Gantt**: il **Gantt** resta la nostra bussola temporale con milestone e dipendenze; **Trello** è lo strumento operativo con cui seguiamo lo sviluppo giorno per giorno. In altre parole, **Scrum è il metodo**, **Trello è il contenitore**: dentro Trello creiamo la board “a colonne”, pianifichiamo gli **sprint di una settimane** (partenza il **lunedì**) e spostiamo le card man mano che avanzano.

Tutto ciò che appare nello **schedula** (il Gantt) **va caricato in Trello**: una card per ogni step del piano. Ogni card contiene:

* **descrizione chiara del task** (cosa deve succedere per dire “finito”),
* **date** coerenti con il Gantt (inizio/fine o almeno una scadenza),
* **chi se ne occupa** (Alex o Alice, o entrambi se serve).

In questo modo possiamo **verificare se il piano viene rispettato** guardando l’avanzamento reale in Trello; se qualcosa slitta lo vediamo subito (la card non è dove dovrebbe essere, o la data è superata) e decidiamo come riassestare il Gantt.

La board Trello usa **cinque colonne** semplici:
**Backlog → Da Fare → In esecuzione → Problemi → Fatto**.
Il flusso “naturale” è Backlog → Da Fare → In esecuzione → Fatto. La colonna **Problemi** non è uno step obbligatorio: è un **parcheggio temporaneo** per le card che hanno un dubbio reale o un ostacolo. Serve a **non perdere di vista i blocchi**: quando spostiamo una card in Problemi, annotiamo *brevemente* che cosa ci frena e rimandiamo ai dettagli (vedi sotto i file dei problemi). Appena il dubbio è chiarito, la card torna in **In esecuzione**.

Il **ritmo** è lineare: lo **sprint** dura **1 settimana**; ogni lunedì e venerdì facciamo un **allineamento** breve. In quell’incontro ciascuno mostra cosa ha implementato, se serve facciamo un po’ di brainstorming, verifichiamo cosa è rimasto indietro rispetto al Gantt, e fissiamo i micro-obiettivi per i giorni successivi. Se emergono ostacoli urgenti, ci sentiamo **ad hoc** alla **prima disponibilità comune**.

Con Trello è possibile visualizzare in maniera semplice e intuitiva lo stato di esecuzione del progetto. 
Per misurare in modo numerico l’andamento rispetto alla pianificazione, ogni venerdì calcoliamo lo **Schedule Performance Index (SPI)**:

SPI = EV / PV
EV (Earned Value): “valore guadagnato”, cioè il lavoro davvero completato fino a oggi, espresso nelle stesse unità della pianificazione (per Ziradò: ore stimate o giorni effettivi da 3h).
→ In Trello: somma dell’Effort (h) delle card spostate in Fatto (o moltiplicate per la % completata, se usiamo il campo “% complete”).

PV (Planned Value): “valore pianificato”, cioè il lavoro che avremmo dovuto completare entro oggi secondo la baseline (Gantt/sprint).
→ In Trello: somma dell’Effort (h) delle card che, da baseline (Sprint/Due date), dovevano essere concluse entro venerdì.

Interpretazione rapida

SPI = 1,00 → in linea con il piano.

SPI > 1,00 → in anticipo (abbiamo completato più di quanto previsto).

SPI < 1,00 → in ritardo (abbiamo completato meno del previsto).

Soglie pratiche: < 0,90: azione correttiva; 0,90–1,10: nella norma; > 1,10: positivo ma verificare che non sia dovuto a stime troppo larghe.

Azioni quando SPI < 1

Spostare fuori sprint i low-priority;

Scomporre card troppo grosse;

Riallocare risorse su percorso critico;

Aggiornare baseline se il cambiamento è approvato (Scope Change).
---

# Issues Log: come li gestiamo davvero

Per i **problemi** adottiamo una doppia traccia molto pratica:

1. **Segnale veloce in Trello**:
   se un task ha un intoppo, **spostiamo la card in “Problemi”** e scriviamo due righe di nota (“che cosa blocca e da quando”). Questo ci dà **visibilità immediata**: è chiaro a colpo d’occhio cosa non sta scorrendo.

2. **Approfondimento nei file personali**:
   i dettagli li conserviamo in due file di testo, **problemiAlice.md** e **problemiAlex.md**. Lì mettiamo le note più lunghe (contesto, tentativi fatti, link utili, ipotesi di fix). È il posto giusto per “pensarci a fondo” senza ingolfare Trello.
   Dalla card Trello possiamo **linkare** la sezione del file corrispondente (es. “Vedi `problemiAlice.md` → #Crash-mappa-Android14”).
   Quando decidiamo insieme cosa fare, la card esce da **Problemi** e rientra in **In esecuzione** o va in **Da Fare** dello sprint successivo (se serve riplanificare). Il problema viene eliminato dal file problemi... e la soluzione adottata viene messa nel file `discussione.md`

Questa soluzione è **coerente** con il nostro modo di lavorare: Trello rimane **leggero e visivo**, i file **problemi*.md** tengono memoria ragionata di ciò che abbiamo scoperto, e in riunione del venerdì possiamo **rivedere rapidamente** la colonna Problemi e, quando serve, aprire i file per capire dove eravamo rimasti.

---


