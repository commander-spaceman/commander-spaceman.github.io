---
title: "Citadel Codex: Markdown Formatting Reference"
description: "A comprehensive guide to all supported text formatting options, styled as an entry from the Citadel Council's official galactic codex."
pubDate: 2026-06-01
---

This document serves as the official formatting reference for all Citadel Codex entries. All contributors must adhere to these standards when submitting species profiles, planetary surveys, and historical records.

## Headings

Codex entries use six levels of section hierarchy:

# H1: Galactic Region

## H2: Star Cluster

### H3: Star System

#### H4: Planet

##### H5: Continent

###### H6: Settlement

---

## Emphasis and Inline Formatting

Species names should be written in **bold** when first introduced. Scientific terminology uses _italics_. Deprecated classifications use ~~strikethrough~~.

Combine them as needed: **_bold and italic_**, ~~**bold strikethrough**~~, ~~_italic strikethrough_~~.

Inline `code` is used for technical identifiers such as `SPECTRE-AUTH-7741` or `relay-314`.

---

## Links

For cross-references, link to other codex entries:

- [Council Species Overview](https://example.com/council-species)
- [Mass Relay Network Map](https://example.com/relay-map "Official Citadel Transit Authority Map")

Autolinked URLs: https://example.com/citadel-archives

---

## Lists

### Unordered: Council Species

- Asari
- Turians
- Salarians

### Nested Unordered: Fleet Composition

- Migrant Fleet
  - Civilian Fleet
    - Liveships
    - Residential vessels
    - Manufacturing ships
  - Heavy Fleet
  - Patrol Fleet

### Ordered: First Contact Protocol

1. Establish communication on standard frequencies
2. Transmit Citadel diplomatic codes
3. Await response for no less than 72 hours
4. If no response, deploy first contact team
5. Document all findings for Council review

### Nested Ordered

1. Primary relay activation
   1. Verify corridor stability
   2. Calibrate field harmonics
   3. Transmit clearance codes
2. Transit execution
   1. Engage drive core
   2. Monitor eezo field coherence
3. Post-transit procedures
   1. Confirm arrival coordinates
   2. Report to relay authority

### Task List: Spectre Mission Checklist

- [x] Receive mission briefing from Council
- [x] Requisition equipment from C-Sec armory
- [ ] Investigate anomalous signals in the Traverse
- [ ] File after-action report
- [ ] Debrief with Councilor Tevos

---

## Blockquotes

> "Stand amongst the ashes of a trillion dead souls and ask the ghosts if honor matters. The silence is your answer."
>
> — Javik, Prothean Warrior

Nested blockquotes for commentary:

> The geth do not intentionally infiltrate Council space.
>
> > This claim has been disputed by multiple Spectre reports filed between 2183 and 2186 CE.
> >
> > > Further investigation recommended. — Office of the Citadel Archivist

---

## Code Blocks

### Sintal (Quarian)

```
process patrol :: cluster.perimeter
  perceive -> sensors.sweep(radius: 500)
  await consensus(cluster.patrol, threshold: 0.8)
    on agree -> navigate target.coordinates
    on disagree -> hold position
  end
end
```

### Python (Alliance Military)

```python
def calculate_barrier_strength(biotic_amp, eezo_charge):
    """Calculate kinetic barrier output for L5n implant."""
    base_field = biotic_amp.power * eezo_charge.density
    resonance = base_field ** 0.73 * BARRIER_CONSTANT
    return min(resonance, MAX_BARRIER_THRESHOLD)
```

### JSON (Citadel Records)

```json
{
  "species": "Quarian",
  "homeworld": "Rannoch",
  "status": "Exiled",
  "population": 17000000,
  "government": "Admiralty Board",
  "council_seat": false
}
```

### Inline Code

Use `getCollection('species')` to query the database. The identifier `SPECIES-QUA-001` refers to the quarian entry.

---

## Tables

### Council Species Comparison

| Species  | Homeworld | Lifespan    | Government        | Council Seat |
| -------- | --------- | ----------- | ----------------- | ------------ |
| Asari    | Thessia   | ~1,000 yrs  | Republics         | Yes          |
| Turian   | Palaven   | ~150 yrs    | Hierarchy         | Yes          |
| Salarian | Sur'Kesh  | ~40 yrs     | Union / Dalatrass | Yes          |
| Human    | Earth     | ~150 yrs    | Alliance          | Yes          |
| Quarian  | Rannoch   | ~150 yrs    | Admiralty Board   | No           |
| Krogan   | Tuchanka  | ~1,000+ yrs | Clan-based        | No           |

### Right-Aligned Numerical Data

| Relay Pair        | Distance (ly) | Transit Time | Efficiency |
| ----------------- | ------------: | -----------: | ---------: |
| Widow → Serpent   |         4,200 |        0.34s |     99.71% |
| Trebia → Parnitha |        12,800 |        1.02s |     99.53% |
| Aethon → Local    |        28,400 |        2.31s |     98.89% |
| Hawking → Far Rim |        64,100 |        5.87s |     96.73% |

---

## Horizontal Rules

Three methods to separate sections:

---

---

---

---

## Images

Images use the standard syntax. If we had access to the Citadel Archives:

![Placeholder description for the Citadel Tower](https://placehold.co/800x400?text=The+Citadel+Tower)

---

## Footnotes

The quarian Migrant Fleet[^1] is the largest concentration of civilian vessels in the galaxy. The fleet's population has remained stable[^2] despite the harsh conditions of permanent spaceflight.

Element zero[^3] remains the foundation of all mass effect technology.

[^1]: Also known as the Flotilla, comprising approximately 50,000 ships.

[^2]: Population estimates range from 15 to 17 million, depending on the source and year of census.

[^3]: Abbreviated as "eezo." A rare material that, when subjected to an electrical current, releases dark energy which can be manipulated into mass effect fields.

---

## HTML Elements

Some formatting requires raw HTML:

<details>
<summary>Classified: Council Eyes Only</summary>

This section contains information classified under Citadel Security Protocol 7. Unauthorized access is a violation of Council law.

The Prothean beacon on Eden Prime contained coordinates to the Conduit, a miniature mass relay connected directly to the Citadel. This information was suppressed by order of the Council in 2183 CE.

</details>

<mark>Highlighted text</mark> is used for critical warnings in official communications.

The chemical formula for eezo-catalyzed reactions: H<sub>2</sub>O + Eezo → H<sub>2</sub>O<sup>+</sup> + e<sup>−</sup>

<abbr title="Special Tactics and Reconnaissance">SPECTRE</abbr> agents operate outside normal legal jurisdiction.

<kbd>Ctrl</kbd> + <kbd>Shift</kbd> + <kbd>T</kbd> opens the tactical overlay on Alliance combat interfaces.

---

## Definition List

<dl>
<dt>Element Zero (Eezo)</dt>
<dd>A rare material capable of generating mass effect fields when exposed to electrical current.</dd>

<dt>Mass Relay</dt>
<dd>A network of Prothean-built devices that enable near-instantaneous faster-than-light travel between star systems.</dd>

<dt>Biotics</dt>
<dd>The ability of certain organisms to generate mass effect fields using eezo nodules embedded in their nervous system.</dd>
</dl>

---

## Escaping Characters

Special characters that require escaping in codex entries:

\*Not italic\* and \*\*not bold\*\*

Use backslashes: \` \~ \# \> \| \[ \]

---

## Combined Formatting

> ### Mission Brief: Priority Alpha
>
> **Objective:** Locate and retrieve Prothean artifact from dig site on `PLANET-EDEN-PRIME`.
>
> _Personnel:_
>
> 1. Commander Shepard — **Team Lead**
> 2. Lt. Kaidan Alenko — _Biotic Support_
> 3. Gunnery Chief Ashley Williams — ~~Reserve~~ Active Duty
>
> | Phase    | Status      | Notes                   |
> | -------- | ----------- | ----------------------- |
> | Recon    | Complete    | No hostiles detected    |
> | Approach | In Progress | Geth presence confirmed |
> | Extract  | Pending     | Beacon status unknown   |
>
> **Warning:** This mission has been flagged as `HIGH RISK` by Alliance Command.
>
> — _Codex Entry Updated: June 2186 CE_

---

_This document is maintained by the Office of the Citadel Archivist. For corrections or additions, contact `archives@citadel.gov`. Last updated: Galactic Standard Date 2186.167._
