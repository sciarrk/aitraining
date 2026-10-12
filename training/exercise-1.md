# Esercizio 1 - Compilare il contesto di progetto

## Scopo

Compilare `.github/copilot-instructions.md` con il contesto AvaRent, affinche' le successive richieste in chat usino lo stesso perimetro. Separare informazioni confermate, ipotesi e dati mancanti senza inventare configurazioni.

Questo e' il primo di otto esercizi da eseguire in ordine. I documenti finali non sono gia' pronti: saranno generati durante il training. La trascrizione fornita per l'esercizio 4 e' interamente fittizia.

## Skill P.R.I.S.M.A.

- `requirements-analysis` (`prisma-functional`): analisi del perimetro e dei requisiti.

## Azioni dell'utente

1. Verifica che i plugin `prisma-functional` e `prisma-core` siano installati e attivi in VS Code. I prompt iniziano con lo slash command della skill.
2. Apri `.github/copilot-instructions.md` e usa una modalita' agente che possa modificare i file del workspace. Copilot carica automaticamente le istruzioni di progetto: non occorre aggiungerle alla chat, nemmeno negli esercizi successivi.
3. Esegui il prompt seguente. Quando l'agente chiede dati non disponibili, rispondi che devono restare `Da confermare`.
4. Esamina il diff: non approvare informazioni inventate e verifica che le linee guida di comportamento esistenti siano preservate.

## Prompt da eseguire in chat

```text
/requirements-analysis

Compila in italiano .github/copilot-instructions.md per il progetto AvaRent,
preservando la struttura e le regole di comportamento esistenti.

AvaRent gestisce oltre 500 community negli USA. Avanade deve realizzare
una soluzione Apartment Management su Dynamics 365 CE/CRM per mantenere
gli appartamenti locati. Il pilota riguarda 5 community del Pacific
Northwest; il rollout nazionale e' successivo e dipende dall'esito del pilota.

Il perimetro comprende prospect e interazioni, inventario e disponibilita',
leasing e liste d'attesa, marketing limitato, onboarding, manutenzione,
import giornaliero, portali candidature e service, approvazioni, sicurezza,
report e soddisfazione tenant. Gli utenti sono dirigenti, manager regionali
e di community, Leasing Agents, tecnici e tenant tramite i portali.
Contrattualistica, pricing e gestione accordi restano al fornitore terzo;
il CRM mantiene i dati operativi necessari a prevedere la disponibilita'.

Vincoli: riparazioni salute/sicurezza entro 24 ore, ricontatto delle liste
d'attesa entro 14 giorni, avvisi a 60/30 giorni dall'uscita programmata.
Lascia Da confermare per ambienti, community nominative, stakeholder,
publisher prefix, solution name, ALM, licenze, KPI e delivery model.
Segnala i dati mancanti. Il brief completo sara' caricato nell'esercizio 2.
```

## Risultato atteso

- `.github/copilot-instructions.md` contiene il contesto AvaRent e mantiene le regole gia' presenti.
- Pilota e rollout nazionale sono distinti; le esclusioni non eliminano i dati operativi necessari.
- Nessun URL, nome di soluzione, licenza o scelta tecnica e' inventato.

## Passo successivo

Prosegui con `training/exercise-2.md`: caricare il caso d'uso originale e convertirlo in Markdown.
