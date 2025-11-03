# RBS – Ziradò  
**(Work Breakdown Structure)**  

> **Commento docente:** RBS e WBS non sono sinonimi. Nel documento di RBS mi aspetto che il focus sia sui requisiti (stati finali attesi) e sulla loro decomposizione gerarchica Requisito → Funzione → Sotto-funzione → Feature. Chiarire se stiamo descrivendo requisiti o attività, evitando ambiguità già dal titolo.

---

## **1. Realizzazione dell’app**

- **Realizzazione mockup** delle varie sezioni.  
- **Implementazione sezioni utente:**
  - **Mappa interattiva:** mappa della città di Cesena con visibili i locali nella loro posizione effettiva.  
  - **Eventi:** lista degli eventi proposti dai locali, ordinati per data.  
  - **Locali:** lista dei locali ordinata per distanza, con possibilità di visualizzare informazioni come giorni di apertura, orari, recensioni, prezzi ed eventuali coupon.  
- **Implementazione sezioni esercente:**
  - **Informazioni attività:** possibilità di modificare i dettagli visibili agli utenti e visualizzare statistiche e recensioni.  
  - **Eventi:** possibilità di aggiungere e modificare gli eventi della propria attività.  
  - **Coupon:** possibilità di aggiungere e modificare i coupon sconto.  
- **Gestione registrazione esercenti:** massimo un account per ogni locale.  
- **Testing** automatici e con utenti reali.  

> **Commento docente:** Qui state descrivendo deliverable e attività tipiche della WBS. Per la RBS mi aspetto requisiti funzionali/non funzionali: es. "L'app deve consentire all'utente di visualizzare la mappa interattiva con geolocalizzazione entro 2 secondi" (misurabile e testabile). Aggiungete i criteri di successo e i parametri di qualità (stabilità, performance, ecc.) per ogni requisito.

---

## **2. Preparazione dei contenuti**

- **Raccolta iniziale dati** di almeno il **75% dei locali del centro**, comprendendo:  
  foto, nome, prezzi indicativi, posizione, orari, giorni di apertura e contatti.  
  (Per “centro” si intende tutta la zona di Cesena non periferica.)  
- **Caricamento** di queste informazioni all’interno dell’app.  

> **Commento docente:** Buona l'indicazione quantitativa (75%), ma specificate come misurate il raggiungimento (es. fonte dati, checklist, soglia di accettazione) e legatelo ai bisogni espressi nelle Conditions of Satisfaction. Serve anche chiarire se questo requisito è stabile o se prevede aggiornamenti periodici.

---

## **3. Ricerca degli sponsor**

- Ricerca di **aziende interessate a sponsorizzare** il progetto.  
- Inserimento di **banner pubblicitari** per gli sponsor all’interno dell’app.  

> **Commento docente:** Mancano gli attributi di valore atteso: qual è il beneficio misurabile (es. coprire il X% dei costi operativi)? Definite metriche di successo e vincoli qualitativi (look & feel dei banner, limiti di intrusività) per renderlo un requisito RBS verificabile.

---

## **4. Lancio e marketing**

- Realizzazione del **logo** e delle **pagine social**.  
- **Pubblicazione** dell’app sugli store (Google Play e App Store).  
- **Campagna pubblicitaria** rivolta sia a utenti che a esercenti, tramite:  
  - social media  
  - manifesti pubblicitari  
  - QR code  
- **Tutorial e spiegazione** dell’app ai locali coinvolti.  

> **Commento docente:** Anche qui ho più attività che requisiti. Per la RBS aspettatevi qualcosa tipo: "Il sistema deve offrire materiali onboarding tali da permettere agli esercenti di completare la configurazione in <30 minuti". Riscrivete in termini di risultati attesi, includendo criteri di misurabilità e testabilità.

---

## **5. Monitoraggio e manutenzione**

- **Sondaggi periodici** per misurare la soddisfazione di utenti ed esercenti.  
- **Inserimento continuo** di nuovi locali in apertura.  
- **Aggiornamenti e manutenzione** tecnica per garantire la stabilità dell’app.  

---

> **Commento docente:** Chiuderei con un nodo di riepilogo che colleghi la RBS ai criteri di successo del progetto e che evidenzi quali requisiti sono ancora incerti (utile per scegliere il PMLC più adeguato). Al momento manca la tracciabilità verso CoS e la dipendenza reciproca con la futura WBS.
