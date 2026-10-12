# Esercizio 3 - Generare le agende dei meeting di analisi

## Scopo

Trasformare il caso d'uso in un piano di analisi con tre meeting, ciascuno con un'agenda salvata in un file distinto. Individuare domande, interlocutori e decisioni da ottenere prima di disegnare la soluzione.

## Skill P.R.I.S.M.A.

- `requirements-analysis` (`prisma-functional`): copertura e qualita' dei requisiti da analizzare.

## Azioni dell'utente

1. Completa l'esercizio 2 e verifica il Markdown del caso d'uso.
2. Aggiungi alla chat `docs/source/avarent-use-case.md`.
3. Esegui il prompt. Non usare la trascrizione dell'esercizio 4 per anticipare le risposte del cliente.
4. Controlla che ogni requisito sia assegnato a un meeting principale, che le dipendenze siano esplicite e che esistano tre file separati.
5. Date e orari qui sotto sono un calendario didattico simulato: non creare inviti reali.

## Prompt da eseguire in chat

```text
/requirements-analysis
Prepara il piano di analisi AvaRent dalla sola docs/source/avarent-use-case.md.
Se manca la fonte convertita, fermati e indica l'esercizio da completare.
Non leggere docs/transcripts/avarent-workshop-01.txt per anticipare le risposte.
Prepara tre incontri simulati su Teams, ciascuno di 90 minuti, 09:00-10:30 Pacific Time:
WS01, 2026-10-12: inventario e processo commerciale; prospect, preferenze, interazioni, disponibilita', liste d'attesa, attribuzione all'agente, Prestige, approvazione tenant, checklist, comunicazioni e portale candidature.
WS02, 2026-10-14: manutenzione ed esperienza tenant; ticket, priorita', SLA riparazione, assegnazione, mobile, approvazione costi, portale tenant, survey, compleanni, high-value e siti personali; dipendenze da WS01.
WS03, 2026-10-16: integrazioni, sicurezza e reporting; import notturno, deduplica, dati del fornitore, ruoli, privilegi distruttivi, sola lettura, filtri community, report e privacy.
Salva tre file distinti:
docs/minutes/agendas/WS01_Leasing-1_Inventario-e-processo-commerciale_20261012-agenda.md
docs/minutes/agendas/WS02_Service-1_Manutenzione-ed-esperienza-tenant_20261014-agenda.md
docs/minutes/agendas/WS03_Cross-1_Integrazioni-sicurezza-reporting_20261016-agenda.md
Assegna tutti i 28 requisiti REQ-01...REQ-28 a un meeting principale e inserisci la mappatura in ciascuna agenda; ammetti richiami secondari.
Indica ruoli da coinvolgere, domande e decisioni da ottenere, dipendenze e timebox che sommino a 90 minuti per agenda.
Evidenzia ambiguita' su scadenza annuale/uscita confermata, giorni/SLA, agente piu' influente, deduplica, privacy, costi > 1000 USD, autenticazione portali e sicurezza iframe; i filtri non sono restrizioni di sicurezza.
Non inventare partecipanti nominativi o risposte, non escludere requisiti dal pilota e non scegliere licenze o moduli senza decisioni esplicite.
Contrattualistica e pricing restano fuori scope; marca le agende come proposte per simulazione formativa, senza creare inviti reali.
Riporta i tre percorsi e verifica copertura e durata; non generare minute o documenti tecnici.
```

## Risultato atteso

- Tre file di agenda in `docs/minutes/agendas/`, non un unico documento cumulativo.
- Tutti i 28 requisiti hanno un meeting principale; nessuno scompare dal piano.
- Ogni agenda dura 90 minuti e contiene domande, non decisioni gia' assunte.

## Passo successivo

Prosegui con `training/exercise-4.md`: generare la minuta del primo workshop.