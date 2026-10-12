# Esercizio 6 - Generare l'FDD dalla minuta

## Scopo

Produrre un Functional Design Document (FDD) in italiano per inventario e processo commerciale, basato su quanto realmente emerso nel WS01. Rendere tracciabili requisiti, decisioni, casi d'uso e criteri di accettazione senza colmare i punti aperti con invenzioni.

## Skill P.R.I.S.M.A.

- `documentation-deliverables` (`prisma-functional`), con il template `functional-analysis-it` incluso nella skill.

## Azioni dell'utente

1. Completa e revisiona gli esercizi 4 e 5. Il DOCX serve per la revisione, ma la fonte da usare in chat rimane il Markdown.
2. Aggiungi caso d'uso Markdown e minuta Markdown alla chat. La trascrizione resta disponibile per risolvere dubbi sull'estrazione.
3. Esegui il prompt. Se vengono chiesti template aziendali o BBP non presenti, indica di segnalarli come mancanti e usare la struttura funzionale della skill per una bozza didattica.
4. Controlla che ogni regola sia supportata dalle fonti o marcata esplicitamente come proposta/ipotesi.
5. Verifica la matrice dei 28 requisiti: quelli non approfonditi devono restare visibili come da analizzare, non sparire o risultare approvati.

## Prompt da eseguire in chat

```text
/documentation-deliverables
Genera in italiano un FDD sul WS01 AvaRent con il template functional-analysis-it.
Fonti: docs/source/avarent-use-case.md e docs/minutes/WS01_Leasing-1_Inventario-e-processo-commerciale_20261012.md; se mancano, fermati.
Consulta docs/transcripts/avarent-workshop-01.txt solo per verificare dubbi sull'estrazione, senza sostituire decisioni della minuta senza evidenza.
Salva docs/specs/avarent-fdd-inventario-leasing.md.
Perimetro: inventario e processo commerciale del pilota di 5 community; contrattualistica, pricing e accordi restano al fornitore terzo, ma i dati operativi per la disponibilita' sono necessari.
Marca il documento Bozza - simulazione formativa - da validare, non un FDD definitivo nazionale.
Descrivi attori, processi, casi d'uso, dati di business e relazioni concettuali, regole, ricerca/disponibilita', liste d'attesa, approvazioni tenant, checklist, interazioni e attribuzione; mantieni parziali Prestige, marketing, portale candidature e dipendenze dall'import. Usa descrizioni testuali, senza diagrammi obbligatori.
Genera user story proposte US-01 e successive, con criteri testabili Dato/Quando/Allora; marca Provvisorio ogni criterio dipendente da un OP irrisolto e collegalo a quell'OP.
Inserisci la matrice di tutti i REQ-01...REQ-28 con fonti, copertura WS01 (analizzato/parziale/da approfondire), decisioni, OP, casi d'uso, story e test intent pertinenti.
I requisiti non trattati restano Da approfondire in WS02/WS03, non Fuori perimetro; non inventare dettagli degli altri workshop.
Mantieni gli ID D-, A- e OP- della minuta e distingui requisiti originali, chiarimenti, decisioni simulate e proposte: non sono approvazioni del documento o legali.
Rendi verificabili 30 vs 31 giorni per la lista d'attesa, ricontatto entro 14 giorni, avvisi a 60/30 giorni e cambio uscita, scadenza annuale non equivalente a unita' libera, preavviso di 30 giorni month-to-month, approvazione prima dell'ingresso e high-value manuale distinto da Prestige.
Lascia aperti calendario/timezone, deduplica, attribuzione all'agente, privacy e compatibilita' dei siti personali dove non definiti.
Se mancano BBP, story approvate o template aziendale, dichiaralo e usa la struttura della skill per la bozza; riporta rischi, dipendenze, ipotesi, copertura e blocchi alla finalizzazione.
Non scegliere moduli, licenze, nomi logici, architettura d'integrazione o implementazioni Dataverse; non aggiornare backlog remoto ne' modificare Dataverse. L'FDD non sostituisce un TDD.
```

## Risultato atteso

- Un FDD in `docs/specs/`, in italiano e coerente con il WS01.
- Matrice completa dei 28 requisiti, con copertura parziale dichiarata e riferimenti verificabili.
- Criteri testabili per quanto concordato; ipotesi e punti aperti non sono decisioni definitive.

## Passo successivo

Prosegui con `training/exercise-7.md`: esportare l'FDD in PDF.