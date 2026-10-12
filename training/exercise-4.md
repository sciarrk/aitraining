# Esercizio 4 - Generare la minuta da una trascrizione

## Scopo

Trasformare una trascrizione in una minuta verificabile: separare discussioni, proposte, decisioni, azioni e punti aperti. Il meeting riguarda inventario e processo commerciale, non l'analisi completa di tutti i requisiti AvaRent.

## Skill P.R.I.S.M.A.

- `documentation-minutes` (`prisma-functional`), con il template italiano `minute-it` incluso nella skill.

## Azioni dell'utente

1. Completa l'esercizio 3.
2. Leggi `docs/transcripts/avarent-workshop-01.txt`, gia' fornito nella repository: persone, dati, date e decisioni sono fittizi.
3. Aggiungi alla chat trascrizione, caso d'uso Markdown e agenda WS01; esegui il prompt.
4. Confronta la minuta con i timestamp della trascrizione. Verifica specialmente la proposta di deduplica sull'email, che non diventa una decisione approvata.
5. Revisiona il file prima dell'export. Non inserire un approvatore reale: la minuta deve restare una bozza didattica da validare.

## Prompt da eseguire in chat

```text
/documentation-minutes
Genera in italiano la minuta WS01 AvaRent con il template minute-it.
Fonte dello svolto: docs/transcripts/avarent-workshop-01.txt.
Usa anche docs/source/avarent-use-case.md e docs/minutes/agendas/WS01_Leasing-1_Inventario-e-processo-commerciale_20261012-agenda.md per confrontare brief e previsto con lo svolto.
Salva docs/minutes/WS01_Leasing-1_Inventario-e-processo-commerciale_20261012.md.
Marca il documento Bozza - simulazione formativa - da validare: nomi e decisioni del training non sono impegni reali.
Preserva data, orario Pacific Time, partecipanti, ruoli, azioni e scadenze della trascrizione.
Distingui conferme, proposte, chiarimenti e correzioni; segnala conflitti e argomenti previsti ma non trattati.
Usa ID stabili D-01, A-01, OP-01 e successivi, con timestamp di provenienza; owner e scadenze assenti restano Da assegnare o Da confermare.
Non attribuire a WS01 approfondimenti di manutenzione, sicurezza o reporting non svolti; WS02/WS03 restano incontri da confermare.
Non inventare gap di prodotto, loghi, firme, approvazioni o decisioni architetturali; segnala asset mancanti del template.
Riporta il file generato, le decisioni estratte e i punti da validare.
```

## Risultato atteso

- Una minuta WS01 in `docs/minutes/`, in italiano e dichiarata fittizia/da validare.
- Decisioni, azioni e punti aperti hanno ID stabili e riferimenti alla trascrizione.
- Owner e scadenze sono fedeli; proposte, dati mancanti e argomenti rinviati non diventano conferme.

## Passo successivo

Prosegui con `training/exercise-5.md`: esportare la minuta in Word.