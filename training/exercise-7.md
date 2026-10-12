# Esercizio 7 - Esportare l'FDD in PDF

## Scopo

Produrre un PDF dell'FDD adatto alla revisione, applicando il template del plugin e verificando leggibilita', impaginazione e integrita' del contenuto.

## Skill P.R.I.S.M.A.

- `convert-to-pdf` (`prisma-functional`): export con template e asset Avanade inclusi nella skill.
- `setup-user` (`prisma-core`): supporto per prerequisiti mancanti, solo se necessario.

## Azioni dell'utente

1. Completa l'esercizio 6 e revisiona l'FDD Markdown.
2. Verifica Pandoc e MiKTeX, come previsto dalla skill. Se il documento contiene Mermaid, verifica anche il filtro e i relativi prerequisiti. Non e' necessario creare diagrammi per questo esercizio.
3. Aggiungi l'FDD alla chat ed esegui il prompt.
4. Apri il PDF e controlla indice, titoli, tabelle, eventuali immagini, numerazione e assenza di tagli. In particolare, verifica la leggibilita' della matrice di tracciabilita'.
5. Se trovi errori, correggi il Markdown o le opzioni di conversione e ripeti l'export. Non modificare il PDF come unica fonte.

## Prompt da eseguire in chat

```text
/convert-to-pdf
Converti docs/specs/avarent-fdd-inventario-leasing.md in docs/specs/avarent-fdd-inventario-leasing.pdf.
Applica il template PDF della skill in italiano, scegliendo un orientamento che renda leggibile la matrice di tracciabilita'.
Conserva contenuto funzionale, ID, decisioni, stato Bozza e simulazione; non dichiarare il documento approvato.
Non alterare il Markdown sorgente e non aggiungere diagrammi, loghi o altri asset assenti nella fonte.
Riporta il PDF realmente creato, il template, i controlli eseguiti e i limiti della verifica visiva, indicando le verifiche manuali necessarie.
```

## Risultato atteso

- Un PDF valido accanto all'FDD Markdown, con contenuto equivalente.
- Tabelle leggibili e nessuna perdita degli ID o dei punti aperti; bozza e simulazione restano riconoscibili.
- Hai completato la verifica visiva; eventuali limiti dell'export sono espliciti.

## Passo successivo

Prosegui con `training/exercise-8.md`: generare il TDD dall'FDD Markdown, non dal PDF.