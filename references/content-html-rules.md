# Content HTML Rules

Questa reference definisce le regole obbligatorie per sviluppare un singolo contenuto SCN.

## Pre-check obbligatorio

Se la lingua non e gia stata specificata, chiedi sempre:

- `In che lingua vuoi che sia scritto il contenuto?`

Non iniziare la stesura senza questa informazione, salvo se la lingua e gia implicita o esplicitata.

## Input consigliati

- page title / topic
- keyword target principale
- eventuali keyword secondarie o query correlate
- primary entity e supporting entities
- page type e query frame
- audience
- destinazione / verticale / brand

## Struttura dell'output

Fornisci sempre, in quest'ordine:

1. `Title Tag:` max 60 caratteri, differenziato dall'H1
2. `Meta description:` max 160 caratteri
3. `HTML body:` senza tag `<html>` o `<body>`
4. `Excerpt:` max 160 caratteri

## Regole editoriali

- Usa un tone of voice simpatico e scherzoso solo nei passaggi narrativi.
- Il paragrafo iniziale deve introdurre prima un contesto naturale, poi integrare la main keyword in modo naturale e grammaticalmente corretto.
- Sotto ogni heading, inizia con una risposta diretta di circa 50 parole.
- In queste porzioni iniziali sotto heading non usare il tone of voice simpatico e scherzoso.
- Usa `H2` e `H3` per strutturare il contenuto.
- Non trasformare tutti gli heading in domande; fallo solo se utile.
- Negli heading non usare tono scherzoso.
- Rispetta la corretta capitalizzazione della lingua.
- Usa la maiuscola a inizio frase.
- Usa liste quando utili, ma evita paragrafi composti solo da elenchi.
- Quando confronti entità o concetti, se opportuno, usa una tabella.
- Le tabelle devono essere mobile-friendly.
- Evidenzia le entita chiave con `<strong>`.
- Evita testo riempitivo.
- Il contenuto deve restare caldo, coinvolgente e non troppo didascalico.

## Regole HTML obbligatorie

Usa solo:

- `<h2>`
- `<h3>`
- `<p>`
- `<ul>`
- `<ol>`
- `<strong>`
- tabelle, solo se utili, nel formato:

```html
<figure class="wp-block-table">
  <table class="has-fixed-layout">
    ...
  </table>
</figure>
```

Non includere:

- `<html>`
- `<body>`

## Sezioni finali obbligatorie

### Summary

Inserisci una sezione denominata `Summary` con massimo 5 punti elenco `<ul>`.

Regole:

- non fare un indice
- fai una sintesi in stile AI Overview
- usa il grassetto per i passaggi chiave
- i punti devono essere informativi e relativamente estesi

### FAQ

Suggerisci almeno 4 FAQ in formato domanda/risposta con risposta contestuale.

Le FAQ:

- non devono necessariamente coincidere con le PAA
- devono essere coerenti con il contenuto
- devono aggiungere utilita reale

## Template operativo

Quando scrivi:

- definisci prima H1 implicito del pezzo
- costruisci una gerarchia H2/H3 coerente con query frame e search intent
- apri ogni sezione con una risposta diretta e pulita
- espandi poi con tono piu caldo e narrativo dove utile
- integra entita, attributi, esempi, confronti, numeri e contesto

## Qualita minima

- nessun keyword stuffing
- nessuna genericita tipo "ci sono molte cose da vedere"
- nessuna risposta vaga priva di soggetto, numero o attributo quando la specificita e importante
- forte coerenza tra keyword target, intent e promessa editoriale
