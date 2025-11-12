# 2201 — Project Definition Statement (PDS) — Ziradò

## 1) Scopo e motivazione

Realizzare un’**app mobile** che unifichi **mappa dei locali e relative informazioni**, **bacheca eventi**, **coupon specific per locale** e **sistema di recensioni** per Cesena, incrementando partecipazione e ricavi degli operatori locali.

**Motivazione**: mancanza di un canale unico affidabile e aggiornato.

## 2) Obiettivi misurabili

* **R1** attiva **entro 31/07/2026**, **R2** entro i 3 mesi successivi al lancio di R!, **R3** entro i 3 mesi successivi a R2.
* **Qualità:** Il tempo di caricamento del 95% delle schermate principali è inferiore a 2 secondi e il tasso di crash per sessione è inferiore all’1%.
* **Adozione:** 5.000 download e rating ≥ 4.0 entro 12 mesi in entrambi gli store di lancio.
* **Ecosistema esercenti:** 75% locali centro storico a 12 mesi.
* **Economia:** break-even di cassa entro 6 mesi dal lancio.

## 3) Scope

* **R1:** Mappa + schede locali, eventi (CRUD, calendario/lista/filtri), login/ruoli, admin, notifiche base, publishing store, requisiti non funzionali.
* **R2:** **Coupon/offerte** e notifiche dedicate.
* **R3:** **Recensioni** (tramite voti o descrizione testuale) con **moderazione** e notifiche correlate.

## 4) Deliverable principali //TODO non sono ovvi?

| **Release** | **Deliverable**            | **Criteri di accettazione**                                                                                                |
| ----------- | -------------------------- | -------------------------------------------------------------------------------------------------------------------------------- |
| R1          | App mobile + backend/admin | Store build approvate; mappa con ≥75% locali; eventi CRUD e filtri; login/ruoli; p95<2s; crash<1%; notifiche testate su 5 device |
| R2          | Coupon + notifiche         | CRUD coupon; consumo in presenza; push entro 5’ dal publish; regression OK                                                       |
| R3          | Recensioni + moderazione   | Voti per tipologia (≥5 domande); testi con segnalazioni; interfaccia admin gestione segnalazioni; regression OK                  |

## 5) Vincoli

* **Tempo:** rispetto del calendario Gantt (documento 2203), periodi **24/12/2025→07/01/2025** e **01/04/2026→08/04/2026** esclusi.
* **Team:** 2 persone, **15 h/sett** ciascuno.
* **Budget diretto:**  circa **404 €**/primo anno + pubblicità di lancio (dettagli nel docuemnto 2205).
* **Store policy/GDPR** obbligatorie per la pubblicazione.

## 6) Assunzioni chiave

* Collaborazione degli **esercenti** per la fornitura e l’aggiornamento dei contenuti.
* Quote **Firebase** e **Mappe** adeguate ai volumi di utenti e dati previsti.
* **Supporto istituzionale minimo** (Comune) per la promozione e la visibilità del progetto.
* **Compatibilità cross-platform** stabile (iOS/Android) garantita dai framework scelti.
* Accesso continuativo agli strumenti di sviluppo (**Firebase, GitHub, IDE, API mappe**) senza interruzioni o modifiche di licenza.
* Permanenza dei membri del team: **Alex e Alice** restano attivamente coinvolti per l’intera durata del progetto.

## 7) Stakeholder e governance

| **Ruolo**                       | **Nome**  | **Responsabilità**                      |
| ------------------------------- | --------- | --------------------------------------- |
| **PM / Responosabile Frontend**      | **Alex**  | Piano, scope, UX, store, sponsor/social |
| **Tech Lead / Responsabile Backend** | **Alice** | Architettura, sicurezza, API, build     |
| **Esercenti pilota**            | — | Dati locali, eventi, coupon             |
| **Sponsor/Comune**              | Comune di Cesena       | Co-marketing, visibilità                |
| **Utenti finali**               | —         | Feedback, rating store                  |

**RACI sintetico**

| **Attività**             | **R** | **A** | **C**     | **I**     |
| ------------------------ | ----- | ----- | --------- | --------- |
| Pianificazione e obiettivi del progetto | Alex            | Alex                 | Alice                | Sponsor                     |
| Struttura tecnica e sicurezza           | Alice           | Alice                | Alex                 | —                           |
| Grafica, interfaccia e contenuti        | Alex            | Alex, Alice                 | Esercenti            | Utenti                      |
| Pubblicazione sugli store               | Alex            | Alex                 | Alice                | Sponsor, Esercenti                     |
| Comunicazione e social media            | Alex            | Alex                 | Sponsor, Alice             | Esercenti                   |
| Regole sulla privacy e GDPR             | Alice            | Alex                | —                    | Sponsor                     |

*(A=Approva · R=Responsabile · C=Consultato · I=Informato)*

## 9) Piano temporale e milestone

| **Milestone**               | **Data**       |
| --------------------------- | -------------- |
| Start R1                    | 01/12/2025     |
| Feature complete R1         | 20/06/2026     |
| Go-Live R1 (store approved) | **31/07/2026** |
| Start R2                    | 01/08/2026     |
| Go-Live R2                  | 16/09/2026     |
| Start R3                    | 15/10/2026     |
| Go-Live R3                  | 30/11/2026     |


// TODO - elimino i successivi? 

## 10) Qualità e accettazione

* **SLO**: p95<2s; crash<1%; push entro 5’.
* **Test**: smoke + regression per release; **RBS.8.1–8.2**.
* **UAT**: gruppo pilota (≥20 esercenti + 30 utenti) prima della submission.
* **Accessibilità**: WCAG 2.1 AA su viste principali.

## 11) Compliance e privacy

* **GDPR**: consensi espliciti, informative trasparenti, DPA con fornitori; data minimization; diritto all’oblio.
* **Store**: conformità linee guida App Store/Google Play; age rating; privacy nutrition labels.
* **Log & audit** per azioni di admin/moderazione.

## 12) Comunicazione e reporting

* **Stand-up** settimanale (30’) e **Review** bisettimanale (60’).
* **Report mensile**: avanzamento, rischi (2206), budget (2205), metriche.
* **Canali**: repo + board Kanban + drive condiviso.

## 13) Budget e procurement

* **Diretti:** 404 € (dev account, dominio, hosting base) + ADV lancio (150 €).
* **Valorizzazione lavoro founder:** 19.575 € (non cassa).
* **Procurement:** account developer, dominio, servizi cloud (quota monitorata).

## 14) Gestione cambi (Change Control)

* **Scope Change Request** **(Form 2303)**: descrizione, beneficio, impatto su tempi/costi/qualità, approvazione PM.
* Solo **Must/Should** per la release corrente; il resto in backlog R+1.

## 15) Metriche di successo (KPI)

* **Adozione:** download, utenti attivi D1/D7/D30.
* **Qualità:** crash rate, p95, errori API.
* **Contenuti:** # eventi/mese, % schede complete.
* **Business:** ricavi sponsor/ADV, CTR push, lead generati.

