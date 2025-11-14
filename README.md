# pm-MastrilliSiroli

Questo repository contiene tutta la documentazione del progetto **Ziradò**, strutturata per poter pubblicare rapidamente un sito statico con GitHub Pages.

## Struttura
- `docs/`: sito statico pronto per GitHub Pages (configurazione Jekyll minima, pagine principali e allegati).
  - `attachments/`: copia in sola lettura dei documenti approvati che vengono citati nel sito (`POS`, `RBS`, `WBS`, ecc.).
- `1_Descrizione_Approccio/` e `2_Documentazione_Progetto/`: workspace sorgente dove continuare a lavorare sulle versioni editabili dei documenti.
- `Checklist_Documenti.md`: elenco dei deliverable previsti.

## Abilitare GitHub Pages
1. Apri **Settings → Pages** nel repository.
2. In **Build and deployment** seleziona `Deploy from a branch`.
3. Imposta **Branch** = `main` e **Folder** = `/docs`.
4. Salva: GitHub pubblicherà il sito all'indirizzo `https://alexsiroli.github.io/pm-MastrilliSiroli/`.

Ogni cambiamento fatto nella cartella `docs/` verrà pubblicato automaticamente dopo il push.
