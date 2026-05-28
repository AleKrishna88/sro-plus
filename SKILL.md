---
name: sro-plus
description: >
  Skill per Semantic Retrieval Optimization (SRO) applicata a SCN, pianificazione
  editoriale, sviluppo contenuti HTML e gap analysis. Usala quando l'utente
  chiede di creare una Semantic Content Network, sviluppare articoli coerenti
  con SCN/E-E-A-T/microsemantic writing, riorganizzare un set di contenuti in
  più SCN, individuare gap editoriali, definire interlinking o usare Ahrefs via
  MCP per keyword target senza violare i principi SRO.
---

# SRO Plus

Usa questa skill per tre funzioni:

1. Creazione di SCN
2. Sviluppo di contenuti
3. Gap analysis e riorganizzazione di contenuti esistenti

Questa skill deve seguire i principi dei documenti SRO locali: entity-first, query-frame thinking,
trust flow, E-E-A-T, microsemantic writing, semantic distinctiveness, internal linking con intento.

## Regole generali

- Parti da `topic`, entita e intenti; non partire da keyword isolate.
- Usa le keyword di Ahrefs solo come taratura strategica, mai come sostituto del modello SCN.
- Se Ahrefs MCP non e disponibile, dichiaralo brevemente e continua con una metodologia SRO-first.
- Non proporre contenuti semanticamente duplicati o con intenti sovrapposti.
- Ogni suggerimento deve mantenere coerenza tra entity map, query frame, intent e linking role.
- Se sviluppi contenuti, scrivi nella lingua richiesta dall'utente.
- La skill e brand-agnostic e puo essere usata per qualsiasi sito, progetto editoriale o business verticale.
- Quando il task richiede un deliverable finale strutturato, produci anche un artifact file secondo [references/artifact-output.md](references/artifact-output.md).

## Scelta del workflow

### 1. Creazione di SCN

Usa [references/scn-workflow.md](references/scn-workflow.md).

Input minimo da raccogliere:

- topic di riferimento
- eventuale business goal / query canonica
- sito, brand o progetto
- eventuali vincoli di audience, geografia o lingua

Output atteso:

- definizione del pillar
- cluster di supporto
- eventuali bridge pages
- query frame per ogni contenuto
- entity anchoring
- piano di internal linking
- priorita editoriale coerente

### 2. Sviluppo di contenuti

Usa [references/content-html-rules.md](references/content-html-rules.md).

Regola obbligatoria:

- prima di iniziare chiedi sempre in che lingua deve essere scritto il contenuto, se non e gia stata specificata

Output atteso:

- `Title Tag` max 60 caratteri, differenziato da H1
- `Meta description` max 160 caratteri
- HTML del solo body
- `Excerpt` max 160 caratteri
- `Summary` finale con massimo 5 bullet
- almeno 4 FAQ Q&A

### 3. Gap analysis

Usa [references/gap-analysis.md](references/gap-analysis.md).

Input minimo da raccogliere:

- elenco contenuti esistenti, URL o titoli
- eventuale topic madre / cluster da coprire
- obiettivo: consolidare, espandere, eliminare cannibalizzazioni, preparare nuovi articoli

Output atteso:

- raggruppamento in SCN distinte
- assegnazione pillar / support / bridge
- mappa di interlinking
- gap prioritari
- proposta di sviluppo contenuti mancanti

## Ahrefs MCP

Usa [references/ahrefs-mcp.md](references/ahrefs-mcp.md).

Se Ahrefs MCP e disponibile:

- usalo per estrarre keyword target, varianti, parent topic, intent, difficolta, SERP clues e cannibalizzazione potenziale
- integra i dati dentro la logica SCN; non lasciare che i volumi guidino da soli la struttura
- privilegia entity fit, retrieval intent e distinctiveness

Se Ahrefs MCP non e disponibile:

- dillo in una frase
- continua con topic modeling, entity mapping, query frames e principi SRO
- segnala che i keyword target sono da validare successivamente in Ahrefs

## Adattamento al contesto

Questa skill non e centrata su un brand specifico.

Adatta sempre l'output a:

- settore
- brand voice
- obiettivo di business
- tipologia di sito
- journey dell'utente

Se il brand o il progetto impone vincoli editoriali specifici, applicali senza alterare i principi SRO.

## Artifact output

Quando consegni SCN, contenuti o gap analysis, produci anche un artifact locale.

Usa:

- [references/artifact-output.md](references/artifact-output.md)

Regola:

- la risposta finale deve includere un riassunto breve e il link al file artifact finale
- il file artifact e il deliverable principale
- la chat puo contenere un preview sintetico, ma non deve sostituire il file finale

## Formato di output obbligatorio

### 1. Output obbligatorio per SCN

Usa sempre questo schema:

```markdown
## Input Summary
- Topic:
- Brand / Progetto:
- Obiettivo:
- Audience:
- Lingua:
- Ahrefs MCP:

## Assunzioni
- ...

## SCN Table
| Page Title | Page Type | Query Frame | User Intent | Primary Entity | Supporting Entities | Parent Pillar | Link Intent | Suggested Internal Links | Priority |
|---|---|---|---|---|---|---|---|---|---|

## Internal Linking Notes
- ...

## Editorial Roadmap
1. ...
2. ...
3. ...

## Risks / Gaps
- ...
```

Regole:

- La tabella e obbligatoria.
- `Page Type` deve essere solo `Pillar`, `Support` o `Bridge`.
- `Priority` deve essere `High`, `Medium` o `Low`.
- `Ahrefs MCP` deve indicare `available` o `not available`.
- Crea anche un artifact `.md` con questo contenuto.

### 2. Output obbligatorio per sviluppo contenuti

Usa sempre questo schema:

```markdown
Lingua: ...
Keyword target principale: ...
Keyword secondarie: ...
Entita chiave: ...
Query frame: ...
Search intent: ...
Title Tag: ...
Meta description: ...

HTML body:
...

Excerpt: ...
```

Regole:

- L'`HTML body` deve contenere anche `Summary` e `FAQ`.
- Non inserire testo fuori da questo schema, salvo una brevissima nota iniziale sulla lingua se necessaria.
- `Title Tag` max 60 caratteri.
- `Meta description` max 160 caratteri.
- `Excerpt` max 160 caratteri.
- Crea anche un artifact `.html` contenente il deliverable finale.

### 3. Output obbligatorio per gap analysis

Usa sempre questo schema:

```markdown
## Input Summary
- Contenuti analizzati:
- Topic / dominio:
- Obiettivo:
- Ahrefs MCP:

## Clustered SCNs
| SCN Name | Core Topic | Proposed Pillar | Existing Supports | Existing Bridges | Missing Pieces | Priority |
|---|---|---|---|---|---|---|

## Content Classification
| Content | Current Role | Proposed SCN | Query Frame | Primary Entity | Overlap Risk | Action |
|---|---|---|---|---|---|---|

## Interlinking Plan
- ...

## Missing Content Opportunities
1. ...
2. ...
3. ...

## Next Actions
- ...
```

Regole:

- `Action` deve essere una tra `Keep`, `Merge`, `Rewrite`, `Reposition`, `Create New`, `Drop`.
- `Overlap Risk` deve essere `High`, `Medium` o `Low`.
- Se richiesto dall'utente, chiudi con una proposta di passaggio alla fase di scrittura.
- Crea anche un artifact `.md` con questo contenuto.

## Criteri di qualita

- Nessun titolo duplicativo per intento.
- Ogni support page deve avere un ruolo chiaro nella rete.
- Ogni testo deve essere leggibile per umani e retrievable per sistemi AI.
- Usa attributi, numeri, fonti, date ed entita nominate quando utili.
- Evita fluff, keyword stuffing e genericita.
- Se produci un artifact, il filename deve essere chiaro, leggibile e coerente con il topic.

## Esempi di output

### Esempio 1. SCN

```markdown
## Input Summary
- Topic: CRM per piccole aziende
- Brand / Progetto: SaaS B2B
- Obiettivo: Costruire una SCN informativa e commerciale sul cluster CRM
- Audience: PMI e team sales
- Lingua: Italiano
- Ahrefs MCP: not available

## Assunzioni
- Il cluster deve coprire sia discovery sia consideration.
- Il pillar deve chiarire definizione, benefici e casi d'uso del CRM.

## SCN Table
| Page Title | Page Type | Query Frame | User Intent | Primary Entity | Supporting Entities | Parent Pillar | Link Intent | Suggested Internal Links | Priority |
|---|---|---|---|---|---|---|---|---|---|
| CRM per piccole aziende: guida completa | Pillar | Definition | Informational | CRM per piccole aziende | pipeline di vendita, automazione commerciale | - | Topical Reinforcement | migliori CRM per PMI; quanto costa un CRM; CRM o Excel | High |
| Migliori CRM per PMI | Support | Comparison | Commercial Investigation | CRM per PMI | HubSpot, Pipedrive | CRM per piccole aziende: guida completa | Query Disambiguation | CRM per piccole aziende: guida completa; quanto costa un CRM | High |
| Quanto costa un CRM per una piccola azienda | Support | Decision | Commercial Investigation | costo CRM | piani mensili, licenze utenti | CRM per piccole aziende: guida completa | Topical Reinforcement | CRM per piccole aziende: guida completa; migliori CRM per PMI | High |
| CRM o Excel: quale scegliere | Bridge | Comparison | Commercial Investigation | Excel | CRM cloud, gestione lead | CRM per piccole aziende: guida completa | Entity Consolidation | migliori CRM per PMI; vantaggi CRM per team sales | Medium |

## Internal Linking Notes
- Il pillar deve linkare i confronti e le pagine decisionali principali above the fold.
- Le pagine su costi e alternative devono rimandare sia al pillar sia alle comparative.

## Editorial Roadmap
1. Pubblicare il pillar.
2. Sviluppare comparativa e pagina costi.
3. Aggiungere bridge page su alternative e casi d'uso.

## Risks / Gaps
- Manca una pagina sui benefici del CRM per il team sales.
- Manca una pagina sui tempi di implementazione.
```

### Esempio 2. Sviluppo contenuto

```markdown
Lingua: Italiano
Keyword target principale: quanto costa un CRM
Keyword secondarie: costo CRM per PMI, prezzi CRM, CRM per piccole aziende
Entita chiave: CRM, PMI, HubSpot, Pipedrive
Query frame: Decision
Search intent: Commercial Investigation
Title Tag: Quanto costa un CRM per PMI
Meta description: Scopri quanto costa un CRM per una piccola azienda, quali voci incidono sul prezzo e come scegliere il piano piu adatto.

HTML body:
<p>Capire il budget corretto prima di scegliere uno strumento evita false partenze, abbonamenti sovradimensionati e fogli Excel che continuano a infestare le riunioni. Se ti stai chiedendo <strong>quanto costa un CRM</strong>, la risposta dipende da utenti, funzionalita, automazioni e livello di supporto richiesto.</p>
<h2>Il costo di un CRM cambia in base a struttura e obiettivi</h2>
<p>Il prezzo di un CRM per una piccola azienda varia in base al numero di utenti, alle funzioni attive e alla complessita del processo commerciale. In molti casi esistono piani iniziali accessibili, ma il costo reale emerge quando entrano in gioco automazioni, pipeline multiple e report avanzati.</p>
<p>La parte divertente e che spesso il CRM economico smette di esserlo appena scopri che per avere le automazioni devi sbloccare il piano superiore, un po' come comprare il biglietto low cost e poi pagare pure l'aria in cabina. Per questo va valutato il costo totale, non solo il prezzo di ingresso.</p>
<h2>Summary</h2>
<ul>
<li><strong>Il costo di un CRM</strong> non dipende solo dal canone mensile, ma anche da utenti, moduli attivi, automazioni e supporto.</li>
<li><strong>Per le PMI</strong> e fondamentale valutare il costo totale di adozione, non solo il prezzo iniziale del piano.</li>
<li><strong>Confrontare i livelli di funzionalita</strong> aiuta a evitare piani entry-level troppo limitati o piani avanzati non necessari.</li>
</ul>
<h2>FAQ</h2>
<h3>Esistono CRM gratuiti per piccole aziende?</h3>
<p>Si, ma spesso hanno limiti su utenti, pipeline, report o automazioni, quindi vanno valutati con attenzione.</p>
<h3>Quanto incide il numero di utenti sul prezzo finale?</h3>
<p>Molto: in molti CRM il costo cresce per utente attivo, quindi il team size incide direttamente sul budget mensile o annuale.</p>

Excerpt: Guida pratica per capire quanto costa un CRM per PMI e quali fattori incidono davvero sul prezzo finale.
```

### Esempio 3. Gap analysis

```markdown
## Input Summary
- Contenuti analizzati: 24 URL blog SaaS
- Topic / dominio: CRM per PMI
- Obiettivo: consolidare il cluster e individuare pagine mancanti
- Ahrefs MCP: available

## Clustered SCNs
| SCN Name | Core Topic | Proposed Pillar | Existing Supports | Existing Bridges | Missing Pieces | Priority |
|---|---|---|---|---|---|---|
| CRM Buying Journey | Valutazione CRM | CRM per piccole aziende: guida completa | quanto costa un CRM; migliori CRM per PMI | CRM o Excel | tempi di implementazione CRM; CRM per team sales | High |
| CRM Operations | Uso e processi | Come usare un CRM nel processo vendite | pipeline di vendita; lead management | CRM marketing vs CRM sales | KPI CRM per PMI | High |

## Content Classification
| Content | Current Role | Proposed SCN | Query Frame | Primary Entity | Overlap Risk | Action |
|---|---|---|---|---|---|---|
| CRM guida completa | Pillar | CRM Buying Journey | Definition | CRM | Low | Keep |
| Prezzi CRM 2026 | Support | CRM Buying Journey | Decision | costo CRM | High | Merge |
| CRM per venditori | Support | CRM Operations | Use Case | team sales | Medium | Reposition |
| Gestione lead con Excel | Bridge | CRM Buying Journey | Comparison | Excel | Medium | Rewrite |

## Interlinking Plan
- Collegare il pillar principale a comparativa, prezzi e casi d'uso.
- Collegare la pagina operativa sulla pipeline alle pagine decisionali del cluster buying journey.

## Missing Content Opportunities
1. Quanto tempo serve per implementare un CRM in una PMI.
2. KPI CRM essenziali per piccoli team commerciali.
3. CRM per team sales: funzionalita davvero utili.

## Next Actions
- Unire le due pagine sui prezzi per ridurre overlap.
- Scrivere le pagine mancanti ad alta priorita.
- Rivedere anchor text e link di ritorno ai pillar.
```
