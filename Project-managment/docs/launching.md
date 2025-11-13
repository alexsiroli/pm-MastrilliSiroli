# **Launching / Execution — Ziradò**

## **Launching**

Definiti **scopo, requisiti e piano**, il team è pronto per la fase di *launching*. 

## **Kick-off meeting**

Viene indetto un **kick-off metting** con lo scopo di definire una matrice di assegnazione delle responsabilità e discutere delle modalità operative del team. 


**Esito:** 
Viene prodotta la seguente roadmap. I *rappresentanti utenti* sono i tre gestori che erano stati contattati sin dalla parte iniziale del progetto.

| **Attività**                                                | **Alex (PM)**                 | **Alice**                     | **Rappresentanti utenti** |
| ----------------------------------------------------------- | ----------------------------- | ----------------------------- | ------------------------- |
| 1. Avvio del progetto                                       | **Responsible**               | Informed                      | Informed                  |
| 2. Configurazione workspace (repo, CI/CD, Trello)           | **Accountable**               | **Responsible**               | Informed                  |
| 3. Modulo **Mappa**                                         | **Accountable**               | **Responsible**               | Consulted                 |
| 4. Modulo **Eventi**                                        | **Accountable**               | **Responsible**               | Consulted                 |
| 5. Modulo **Coupon/Offerte**                                | **Accountable**               | **Responsible**               | Consulted                 |
| 6. **Sistema Notifiche**                                    | **Accountable**               | **Responsible**               | Consulted                 |
| 7. **Backend/API & Admin**                                  | Consulted                     | **Accountable / Responsible** | Informed                  |
| 8. **Frontend/UI**                                          | **Accountable / Responsible** | Consulted                     | Consulted                 |
| 9. **QA & Hardening** (performance, privacy, accessibilità) | **Accountable**               | **Responsible**               | Consulted *(UAT)*         |
| 10. **Lancio/Go-Live**                                      | **Accountable**               | **Responsible**               | Informed                  |
| 11. **Consegna progetto** (deliverable finali)              | **Responsible**               | Informed                      | Informed                  |
| 12. **Gestione cambiamenti di scope**                       | **Accountable**               | Consulted                     | Consulted                 |
| 13. **Modulo Prenotazioni** *(Scope change 2303)*           | **Accountable**               | **Responsible**               | Consulted                 |

## Legend
- Responsible (R): Persona(e) responsabile dell’attività e del suo completamento consuccesso.
- Accountable (A): Persona(e) Incaricato dell’approvazione del risultato dell’attività.
- Supporting (S): Risorsa(e) assegnata per supportare il responsabile.
- Consulted (C): Persona(e) disponibile per assistere il responsible.
- Informed (I): Persona(e) membro che deve essere tenuto informato sullo stato di avanzamento.
---

## **Regole operative per il team**

Per garantire un corretto svolgimento delle attività e una comunicazione efficiente tra i membri del team, sono state definite le seguenti regole operative:
### **Tools**

* **Task management:** la gestione delle attività viene gestita tramite **Trello**, che permette di segnare le singole attività come **card** da spostare nelle diverse colonne (*Backlog → Da fare → In esecuzione → Problemi → Fatto*).
  Ogni task ha **owner**, **data di inizio**, **data di fine** **breve descrizione con riferimento alla WBS associata**. In caso di problemi o dubbi durante l'esecuzione del task, questo viene spostato in Trello nella colonna dei problemi. Una descrizione più approfondita del problema in questione viene descritta dallo sviluppatire all'interno del file **`problemiAlice.md`** / **`problemiAlex.md`**.

* **Version control:** 
si lavora in una repo condivisa su **GitHub** con **feature branches + Pull Request**; **CI/CD (GitHub Actions)** verso *staging* e *prod*; test automatici su PR.

* **Comunicazioni:** per le comunicazioni, è previsto l'utilizzo di chat informali, come **WhatsApp** o **Telegram**. Si predilige comunque un incontro in presenza qualora bisogna discutere di questioni più complesse.  

### **Meetings**
Sì, ha senso parlarne—ma ti conviene **allineare i nomi agli eventi Scrum** e precisare la cadenza. Ti propongo questo testo “pronto da incollare”:

### **Meetings (Scrum adattato)**

Adottiamo Scrum, con sprint di 1 settimana (lun–ven).

* **Sprint Planning — lunedì (30–45’)**

  * Definizione dello **Sprint Goal**, selezione dallo **Sprint Backlog**, stima rapida e assegnazioni.
* **Sprint Review — venerdì ore 10:00 (20–30’)**
  * Allineamento e discussione su quanto svolto durante la settimana, controllo dei tempi tramite schedula. 

* **Ad-hoc meetings**

  * Convocati alla **prima disponibilità comune** per urgenze o decisioni bloccanti.



---

## **Problem solving**

Il team adotta un approccio collaborativo per risolvere i problemi basato sulla regola dei 5 punti di Daniel Couger:
1. **Definizione del problema**: chi lo rileva descrive *cosa/dove/quando*.
2. **Analisi cause**: il team mira a identificare le cause principali del problema. 
3. **Generazione idee**: il team propone un'ampia gamma di soluzioni al problema presente.
4. **Valutazione & priorità**: sulla base di fattori come impatto, sforzo, rischio e urgenza, si classificano le diverse soluzioni proposte per determinare quale sia la più efficace.
5. **Piano d’azione**: si decide come implementare la soluzione scelta: chi fa cosa e in quanto tempo. Allineamento con Trello.
Al termine dello sviluppo della soluzione, si prevede un meeting per commentare il risultato ottenuto. Se non soddisfacente, si torna al punto 2.
---

## **Decision making & consenso** 
L'approccio di decision making che si segue è **collaborativo**: tutte le decisioni vengono prese insieme da Alex e Alice.
Ogni decisione va registrata in un apposito file chiamato **`DECISION.md`** (contesto, opzioni considerate, scelta e motivazione).
Se non c’è accordo**, si attiva **Conflict Resolution**.

## Conflict Resolution

Quando c’è disaccordo su una decisione/soluzione, o mancano competenze:
1. Confronto focalizzato Alex–Alice (max 30’).
2. Parere terzo o AI: in base al tema, si può chiedere l’opinione di un conoscente competente, di un docente/professionista o consultare uno strumento di AI per alternative/analisi aggiuntive.
3. Rivalutazione con i nuovi elementi.
4. Si procede solo se Alex e Alice concordano.

---

## **Gestione cambiamenti di scope**

In data 15/02/2026, durante lo sviluppo della sezione eventi, Alice pensa che si potrebbe aggiungere una sezione **Prenotazioni** per permettere agli utenti di prenotarsi ad un evento. Al fine di documentare questa idea, redige il seguente **Scope Change Request Form**.

📂 **Allegato:** **Scope Change Request Form** è riportata nell’**Allegato 5**.

Viene quindi indetta una riunione con Alex in cui si discute dell'impatto di questa modifica all'interno del progetto, racchiuso nel seguente documento.

📂 **Allegato:** **Project Impact Statement** è riportata nell’**Allegato 6**.

Alla luce dei numerosi benefici, Alex decide di approvare la proposta e firma il **Scope Change Request Form** in data 01/03/26. Viene quindi allineato lo schedula.
