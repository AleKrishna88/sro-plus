# Artifact Output

Questa reference definisce come consegnare i deliverable finali in formato artifact file.

## Principio

Ogni deliverable importante deve esistere anche come file locale finale.

La chat serve per:

- raccogliere input
- spiegare assunzioni
- dare un breve riepilogo

Il file artifact serve per:

- consegna
- riuso
- revisione
- handoff

## Directory consigliata

Salva gli artifact in una cartella locale chiamata `artifacts/` nella workspace corrente, salvo istruzioni diverse dell'utente.

## Formati per funzione

### SCN

- formato file: `.md`
- nome consigliato: `<topic-slug>-scn.md`

### Sviluppo contenuti

- formato file: `.html`
- nome consigliato: `<topic-slug>.html`

### Gap analysis

- formato file: `.md`
- nome consigliato: `<topic-slug>-gap-analysis.md`

## Struttura della risposta finale

La risposta finale deve contenere:

1. breve sintesi del risultato
2. link Markdown al file artifact finale

Esempi:

- `[SCN Giappone - giappone-scn.md](/absolute/path/artifacts/giappone-scn.md)`
- `[Quando andare in Giappone - quando-andare-in-giappone.html](/absolute/path/artifacts/quando-andare-in-giappone.html)`

## Regole

- Non linkare file intermedi, bozze o scratch file salvo richiesta.
- Se ci sono piu deliverable finali, linkali separatamente.
- Per i contenuti HTML, il file finale deve contenere il deliverable completo pronto all'uso.
- Se l'utente non chiede esplicitamente solo brainstorming o schema, privilegia la produzione dell'artifact finale.
