# Esercizio 8 - Generare il TDD dall'FDD

## Scopo

Proporre un Technical Design Document (TDD) in italiano per inventario e processo commerciale del pilota AvaRent, traducendo l'FDD in un design implementabile su Dataverse e Power Platform. L'esercizio riguarda l'analisi tecnica, non l'implementazione: scelte proposte, ipotesi e blocchi devono restare distinguibili dai vincoli confermati.

## Skill P.R.I.S.M.A.

- `solution-architecture` (`prisma-functional`), con il template `technical-design-it` incluso nella skill.

## Azioni dell'utente

1. Completa e revisiona gli esercizi 6 e 7. Il PDF serve per la revisione; l'input del TDD resta `docs/specs/avarent-fdd-inventario-leasing.md`.
2. Aggiungi alla chat l'FDD Markdown, la minuta WS01 Markdown e `docs/source/avarent-use-case.md` per i riferimenti alle fonti.
3. Esegui il prompt. Se mancano analisi approvata, ADR, standard di progetto o template aziendale, richiedi una bozza didattica con ipotesi esplicite, senza inventare documenti o approvazioni.
4. Valuta architettura, modello dati, componenti e sicurezza proposti; controlla la tracciabilita' verso REQ, US e OP dell'FDD e che i punti aperti funzionali non diventino decisioni tecniche definitive.
5. Revisiona informazioni Da confermare e blocchi prima di considerare il design implementabile. Non eseguire deploy, codice o modifiche in Dataverse.

## Prompt da eseguire in chat

```text
/solution-architecture
Genera in italiano un TDD con il template technical-design-it, senza eseguire implementazioni.
Input principale: docs/specs/avarent-fdd-inventario-leasing.md, non il PDF; se manca, fermati.
Fonti di riferimento: docs/minutes/WS01_Leasing-1_Inventario-e-processo-commerciale_20261012.md e docs/source/avarent-use-case.md.
Salva docs/specs/avarent-tdd-inventario-leasing.md.
Marca il documento Bozza - simulazione formativa - non approvato.
Limita il design a inventario e processo commerciale WS01 del pilota di 5 community; non estenderlo ai workshop non analizzati.
Descrivi l'architettura proposta su Dataverse e Power Platform in forma testuale; diagrammi non sono necessari.
Proponi il modello dati Dataverse con tabelle, colonne e tipi, relazioni, chiavi e ownership, distinguendo lo schema proposto da eventuali dati esistenti documentati.
Motiva i componenti client/server e le automazioni necessari al perimetro, senza prescrivere componenti non giustificati dall'FDD.
Tratta integrazioni, sicurezza, gestione errori, monitoraggio, performance, test e ALM dove pertinenti.
Mantieni la tracciabilita' a REQ, US e OP dell'FDD: non risolvere punti aperti funzionali inventando un design.
Distingui scelte tecniche proposte, vincoli confermati e ipotesi; evidenzia dipendenze e blocchi alla finalizzazione.
Se mancano analisi approvata, ADR, standard di progetto o template aziendale, dichiarali Da confermare e usa la struttura della skill per la bozza.
Non inventare URL di ambienti, licenze, prefix definitivi, schema esistente, ADR reali, KPI di performance o approvazioni; le informazioni mancanti restano Da confermare.
Non generare codice esecutivo, non eseguire deploy ne' modifiche Dataverse; riporta il file creato, le proposte e i blocchi da revisionare.
```

## Risultato atteso

- `docs/specs/avarent-tdd-inventario-leasing.md` contiene una bozza tecnica significativa, in italiano e non approvata.
- Architettura, modello dati e componenti proposti sono motivati e tracciabili all'FDD per inventario e leasing del pilota di 5 community.
- Vincoli confermati, ipotesi, informazioni Da confermare e OP funzionali restano distinti; i blocchi non sono risolti con dati inventati.
- Nessun deploy, codice esecutivo o modifica Dataverse e' stato effettuato.

## Chiusura del percorso

Verifica di avere:

- Contesto di progetto compilato nell'esercizio 1.
- Originale caricato manualmente e Markdown integrale del caso d'uso.
- Tre agende distinte per WS01, WS02 e WS03.
- Minuta WS01 Markdown e DOCX revisionato visivamente.
- FDD Markdown e PDF revisionato visivamente.
- TDD Markdown revisionato, con scelte proposte e blocchi espliciti.

La trascrizione fittizia resta la fonte dell'esercizio 4. Nessun esercizio richiede un ambiente Dataverse reale o una pubblicazione della soluzione; FDD e TDD restano bozze didattiche, non documenti approvati.