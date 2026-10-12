# Esercizio 5 - Esportare la minuta in DOCX

## Scopo

Produrre una versione Word modificabile della minuta, preservando il contenuto e usando gli stili e il template forniti dal plugin.

## Skill P.R.I.S.M.A.

- `convert-to-docx` (`prisma-functional`): conversione Markdown in Word con gli asset della skill.
- `setup-user` (`prisma-core`): supporto per prerequisiti mancanti, solo se necessario.

## Azioni dell'utente

1. Completa l'esercizio 4 e revisiona la minuta Markdown.
2. Verifica Pandoc. Se sono presenti diagrammi Mermaid, verifica anche i prerequisiti del filtro indicati dalla skill.
3. Aggiungi la minuta alla chat ed esegui il prompt.
4. Apri il DOCX con Word o un lettore compatibile: controlla titoli, tabelle, accenti, eventuali immagini e assenza di tagli. La creazione del file non basta a provare la qualita' visiva.
5. Il Markdown resta la fonte: apporta li' eventuali correzioni e ripeti l'export, senza creare versioni divergenti solo in Word.

## Prompt da eseguire in chat

```text
/convert-to-docx
Converti docs/minutes/WS01_Leasing-1_Inventario-e-processo-commerciale_20261012.md in docs/minutes/WS01_Leasing-1_Inventario-e-processo-commerciale_20261012.docx.
Applica il template DOCX della skill in italiano, con stili Word per i titoli e tabelle editabili.
Conserva integralmente testo, date, owner, ID, stato di bozza e simulazione; non aggiungere firme o approvazioni.
Non alterare il Markdown sorgente e non aggiungere diagrammi o immagini assenti nella fonte.
Riporta il file realmente creato, i controlli eseguiti e le verifiche visive ancora necessarie, senza dichiarare verificata un'impaginazione non esaminata.
```

## Risultato atteso

- Un file DOCX valido accanto alla minuta Markdown, con contenuto equivalente.
- Titoli e tabelle sono modificabili; l'avvertenza di simulazione e' preservata.
- Hai controllato visivamente il risultato; il Markdown originale non e' cambiato.

## Passo successivo

Prosegui con `training/exercise-6.md`: costruire l'FDD dalla minuta Markdown, non dall'export Word.