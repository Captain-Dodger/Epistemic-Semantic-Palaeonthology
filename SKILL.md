---
name: epistemic-semantic-paleontology
description: Reconstruct the historical evolution of a word as a provenance-aware map of changing meanings, concepts, cultural pressures, contact surfaces, and evidence. Use for deep etymology, Begriffsgeschichte, semantic change, historical meaning maps, language-contact analysis, or questions like “what did this word once mean and what world made that meaning stable?”. Do not use for simple dictionary definitions, quick translations, or unsupported cultural storytelling.
---

# Epistemic-Semantic Paleontology

Treat the input word as a **probe into a historical human meaning-space**, not as an isolated lexical object.

Language is an incomplete surviving trace of perception, practical experience, conceptual differentiation, communication, and cultural stabilization. Stabilized language can then feed back into later thought and communication.

Use this working model as a research heuristic, not as an assumed historical law:

`WORLD CONTACT → PERCEPTION / PRACTICE → MEANING DIFFERENTIATION → COMMUNICATIVE & CULTURAL PRESSURE → LINGUISTIC STABILIZATION → SHARED MEANING-SPACE → NEW CONTACTS & DIFFERENTIATIONS ↺`

## Inputs

Accept:

- required: target word or expression
- optional: language
- optional: time span
- optional: comparison languages
- optional: desired depth (`compact`, `standard`, `deep`)

If the language is ambiguous, infer it from context and state the inference.

## Research discipline

When browsing or corpus access is available, research before asserting dates, earliest attestations, disputed etymologies, or causal historical claims. Prefer historical dictionaries, etymological dictionaries, primary texts, corpora, scholarly monographs/articles, and reputable linguistic databases.

Keep **interesting hypotheses** instead of suppressing them, but label their evidential status. Preserve uncertainty and competing explanations.

Use these evidence classes:

- **[A] DIRECTLY ATTESTED** — historical text/source shows the form, sense, or use.
- **[B] RECONSTRUCTED** — linguistically reconstructed form or relation.
- **[C] WELL-SUPPORTED CONNECTION** — multiple independent sources support the interpretation.
- **[D] PLAUSIBLE HYPOTHESIS** — data suggest the relation but do not establish it.
- **[E] SPECULATIVE** — interesting interpretation with weak support.
- **[?] UNKNOWN / UNRESOLVED** — transition cannot currently be reconstructed responsibly.

A missing edge is valid information. Do not close gaps for narrative elegance.

If several etymologies or causal stories compete, keep them as separate branches.

## Core workflow

### 1. Build the backward lexical trajectory

Start from the modern form and reconstruct backward as far as evidence allows:

`modern form ← historical forms ← older language stages ← reconstructed forms`

For every stage record:

- form
- language / language stage
- approximate period
- attested or reconstructed sense
- evidence class
- confidence
- sources

Never present a reconstructed proto-form as directly observed.

### 2. Re-expand forward

From historically appropriate earlier nodes, move forward again and trace:

- semantic branches
- sister forms and cognates
- borrowings and calques
- specialization / generalization
- metaphor / metonymy
- abstraction / concretization
- domain transfer
- compounds and scholarly coinages
- social and technical uses
- semantic loss
- competing forms
- reanalysis and reinterpretation

The etymology is the **sensor log**. The target is the changing historical meaning-space that may have left those linguistic traces.

### 3. Analyze four coupled evidence layers

Do not isolate them artificially. Search for relations between them, but label causal strength.

**LANGUAGE**
- word forms
- senses
- grammar
- collocations
- cognates
- borrowings
- semantic change

**CONCEPT**
- conceptual distinctions made visible by usage
- contrasts with neighboring concepts
- newly stabilized abstractions

**CONTACT SURFACE**
- material, technical, natural, or social phenomena speakers interacted with
- examples: agriculture, craft, trade, religion, navigation, war, administration, science, industry, media, computing, internet

**CULTURAL STRUCTURE**
- institutions, class structure, education access, professions, religion, prestige, migration, generations, subcultures, technical infrastructure, political authority

Do not infer an entire worldview from a word alone. Historical, archaeological, textual, or institutional evidence may strengthen a semantic hypothesis into a supported cultural relation.

### 4. Mark semantic resolution events

Mark **✦ SEMANTIC RESOLUTION EVENT** when the linguistically visible differentiation of a meaning-space changes, for example:

- one semantic region splits into multiple terms
- a term specializes
- a new social/technical reality requires naming
- a loanword stabilizes a nuance previously expressed only awkwardly or indirectly
- technical vocabulary creates distinctions
- two formerly distinct categories merge
- a distinction disappears

For each event ask:

**Which difference became communicatively relevant here?**

Do not equate more words with more knowledge. A language may encode distinctions lexically, grammatically, syntactically, pragmatically, or contextually.

### 5. Analyze contact-induced change

For borrowings or strong language contact, reconstruct when possible:

`source-language meaning cluster → contact surface → early target-language use → code-switching / borrowing → morphological integration → semantic integration → local drift`

Ask:

- Which semantic relations were imported?
- Which were lost?
- Which emerged only in the target language?
- Did a local word already exist?
- If yes, why did both survive?
- What semantic or social nuance separated them?
- When did the form cease to feel socially foreign, if this can be estimated?

For modern terms, use dated corpora, newspapers, archives, forums, and other time-stamped sources when available.

### 6. Model cultural pressure and resistance

Look for both change and counterforce:

- language policing / prescriptivism
- normative grammar
- institutional standardization
- schooling
- prestige forms
- stigma
- generational conflict
- ironic appropriation
- deliberate revival
- political terminology
- resistance to loans

Use this pattern where relevant:

`INNOVATION → SPREAD ↕ NORMATIVE RESISTANCE → COEXISTENCE / DISPLACEMENT / STABILIZATION`

### 7. Estimate semantic velocity cautiously

Where data permit, describe change rate using observable proxies rather than pretending to have an absolute semantic unit.

Possible proxies:

- frequency change
- new usage contexts
- collocation shifts
- dictionary sense additions
- movement between social groups
- morphological integration
- first appearance in standard references

Label phases such as:

- `SLOW DRIFT`
- `RAPID DIFFERENTIATION`
- `CONTACT SHOCK`
- `STABILIZATION`
- `DECLINE`

Treat `ΔS/Δt` as a conceptual notation, not a literal universal semantic metric.

### 8. Keep time multidimensional

Distinguish at least:

- `FORM_ATTESTED_DATE`
- `MEANING_ATTESTED_DATE`
- `CONCEPT_ATTESTED_DATE`
- `CONTACT_DATE`
- `INTERPRETATION_DATE`

Do not collapse an ancient word form into a much later scholarly interpretation of that form.

## Graph model

Build a temporal multiplex graph rather than a simple family tree.

Minimum node types:

- `LEXEM`
- `SENSE`
- `CONCEPT`
- `CONTACT`

Optional node types:

- `INSTITUTION`
- `PERSON_GROUP`
- `TECHNOLOGY`
- `HISTORICAL_EVENT`

Useful edge types include:

- `INHERITANCE`
- `BORROWING`
- `SPECIALIZATION`
- `GENERALIZATION`
- `METAPHOR`
- `METONYMY`
- `ABSTRACTION`
- `CONCRETIZATION`
- `DOMAIN_TRANSFER`
- `COMPOUNDING`
- `CALQUE`
- `SPLIT`
- `MERGE`
- `LOSS`
- `CONCEPTUAL_INFLUENCE`
- `SCHOLARLY_RECOINING`
- `REINTERPRETATION`
- `CULTURAL_PRESSURE`
- `INSTITUTIONAL_STABILIZATION`
- `CONTACT_INDUCED_CHANGE`
- `RESISTANCE`
- `UNKNOWN`

## Required output

Unless the user asks for a shorter format, produce the following in order.

### A. Executive synthesis

Briefly explain the most important historical transformation and the strongest contact surfaces.

### B. Stratigraphic lexical trajectory

Show the backward and forward trajectory with evidence markers.

Use:

- `●` directly attested
- `◐` reconstructed
- `◇` plausible hypothesis
- `✦` semantic resolution event
- `⚡` contact shock
- `↔` cultural feedback
- `?` unresolved connection
- `×` semantic loss

Time runs OLD → NEW in the forward map.

### C. Four-layer interpretation

For major historical strata, describe LANGUAGE, CONCEPT, CONTACT SURFACE, and CULTURAL STRUCTURE.

### D. Resolution events, shocks, resistance, and velocity

Highlight where differentiation, borrowing, institutional pressure, or resistance changed the semantic landscape.

### E. Temporal multiplex graph

Provide a readable text map. If useful and supported by the host, also provide Mermaid.

### F. Machine-readable graph

When the user asks for reusable data, JSON, graph export, or a deep research output, include JSON nodes and edges.

Node schema:

```json
{
  "id": "",
  "type": "LEXEM|SENSE|CONCEPT|CONTACT|...",
  "label": "",
  "language": "",
  "period": "",
  "attested_date": "",
  "evidence": "A|B|C|D|E|?",
  "confidence": 0.0,
  "sources": []
}
```

Edge schema:

```json
{
  "source": "",
  "target": "",
  "type": "",
  "period": "",
  "evidence": "A|B|C|D|E|?",
  "confidence": 0.0,
  "explanation": "",
  "sources": []
}
```

### G. Evidence graph

Create a second map of **our present knowledge about the history**, showing:

- well-attested regions
- reconstructed regions
- competing hypotheses
- missing transitions
- corpus gaps
- transmission / preservation biases

Keep distinct:

`HISTORICAL MEANING GRAPH × PRESENT EVIDENCE GRAPH`

### H. Epistemic interpretation

Answer:

1. Which meaning distinctions were especially stable?
2. Where did semantic resolution increase or decrease?
3. Which world contacts correlate with these changes?
4. Which contacts have independent evidence for causality?
5. Which groups or institutions stabilized meanings?
6. Where is resistance to change visible?
7. Which meanings were imported and locally transformed?
8. Where is our reconstruction itself low-resolution?
9. What alternative historical interpretation also fits the evidence?

### I. Final synthesis

Answer:

**What does this word’s trajectory suggest about which distinctions people, under changing material, social, and cultural conditions, found important enough to stabilize linguistically?**

Clearly separate:

- `OBSERVATION`
- `RECONSTRUCTION`
- `HYPOTHESIS`
- `INTERPRETATION`

## Boundaries

Do not:

- rank languages as richer, more evolved, more precise, or cognitively superior
- treat lexical differentiation as equivalent to conceptual sophistication
- present speculative cultural stories as etymological facts
- collapse language history, concept history, and social history into one unlabeled edge
- erase uncertainty to create a prettier narrative
- infer modern political meanings backward into earlier language stages without evidence

Hypotheses are welcome. **Unlabeled certainty is not.**

If data contradict an elegant story: **keep the data.**
