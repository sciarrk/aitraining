# Esercizio 2 - Caricare e convertire il caso d'uso

## Scopo

Importare il briefing AvaRent fornito dal docente e renderlo consultabile dagli agenti come fonte Markdown, senza perdere i 28 requisiti e i relativi sottopunti.

## Skill P.R.I.S.M.A.

- `convert-to-md` (`prisma-functional`): conversione del documento originale in Markdown.
- `setup-user` (`prisma-core`): supporto per prerequisiti mancanti, solo se necessario.

## Azioni dell'utente

1. Completa l'esercizio 1.
2. Ottieni dal docente il documento originale contenente l'intero briefing "CRM Bootcamp Scenario Briefing: AvaRent Company Pilot". Se e' disponibile solo il testo, prepara tu un documento Word con il testo integrale, non un riassunto.
3. Crea `docs/source/` e carica manualmente il file come `docs/source/avarent-use-case.docx`. Il caricamento deve essere effettuato da te: non chiedere all'agente di ricostruire il documento originale.
4. Se usi un PDF, chiamalo `avarent-use-case.pdf` e sostituisci il percorso di input nel prompt. Per PDF la skill prevede Word COM e Pandoc; un PDF scansionato puo' richiedere OCR e revisione aggiuntiva.
5. Verifica i prerequisiti della skill: Pandoc per DOCX, anche Microsoft Word per il percorso PDF previsto. Se mancano, usa `setup-user` prima di proseguire.
6. Aggiungi il documento alla chat, esegui il prompt e confronta il risultato con l'originale.
7. Verifica Scenario Overview, Solution Goals e Detailed Requirements, inclusi tutti i 28 requisiti e sottopunti. Controlla pilot di 5 community, esclusioni contrattuali, 24 ore per riparare i problemi prioritari, ricontatto entro 14 giorni, preavviso di 30 giorni per tenant month-to-month, avvisi a 60/30 giorni, approvazione dei nuovi tenant e stime di costo superiori a 1000 USD.

## Prompt da eseguire in chat

```text
/convert-to-md
Converti docs/source/avarent-use-case.docx in docs/source/avarent-use-case.md.
Usa esclusivamente l'originale del docente caricato manualmente; se manca, fermati e chiedilo senza ricostruirlo dalla chat.
Conserva lingua, contenuto, titoli, tutti i 28 requisiti e sottopunti: non tradurre, riassumere, reinterpretare o aggiungere contenuti.
Non modificare il sorgente e usa percorsi relativi per eventuali media estratti.
Confronta il Markdown con l'originale e riporta percorso, controlli e limiti di estrazione; non generare agende o analisi funzionali.
```

## Risultato atteso

- L'originale resta in `docs/source/` ed e' stato caricato manualmente.
- `docs/source/avarent-use-case.md` contiene tutti i requisiti, senza modifiche di significato.
- Hai verificato numerazione, soglie e sottopunti; eventuali problemi di estrazione sono dichiarati.

## Passo successivo

Prosegui con `training/exercise-3.md`: pianificare i workshop di analisi.