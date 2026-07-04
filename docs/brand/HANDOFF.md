# Handoff — Integrate the Hive brand & philosophy

**For:** a local agent picking up Agix work today.
**From:** the ideation session with the Beekeeper (Brandon Lewis).
**Date:** 2026-07-04.
**Source of truth:** [`docs/brand/north-star.md`](./north-star.md) in `agix-ai/.github`
(branch `claude/repository-ideation-atrlg2`). **Read it fully before acting** — this
file is only the action layer on top of it.

---

## 0. TL;DR of what you're integrating

Agix's brand and philosophy is the **hive**. The thesis: *intelligence at scale is
a well-tended colony, not a bigger brain* — emergence over command, stewardship
over control, ownership over rental. The human is **the Beekeeper**, standing
outside the colony (never the queen). The unit of the Agix OS is **one hive = one
project/enterprise**; many hives = the **apiary**. Agents are **castes** (worker,
forager, scout, guard, nurse, builder, drone…). Your job is to make the product,
docs, blogs, visuals, and — where you have the code — the architecture, speak this
language coherently.

## 1. What is DECIDED (treat as locked unless the Beekeeper says otherwise)

- The hive/beekeeper/colony metaphor is the brand's North Star.
- **Beekeeper ≠ Queen.** The human is an external steward. The queen is a
  *coherence signal* (pheromone = durable leadership/north-star), never a commander.
- The **hive is the unit** of the Agix OS (project/contained enterprise); apiary =
  portfolio.
- **Biological honesty is a brand asset.** Drones don't do labor — they cross hive
  boundaries. Use the lexicon in north-star.md §4; don't invent bee-facts.
- **Drone = inter-hive messenger; Guard = inbound authz/inspection.** Together they
  are the inter-hive trust boundary. Cross-hive comms must be secure & auditable.
- Visual direction: **hexagon** primitive (cell = graph node), **honey-amber +
  comb-black** palette — deliberately warm, *not* the default cold AI blue.
- Voice: naturalist-engineer / apiarist field notes. Blog series = **"Field Notes
  from the Hive."**

## 2. What is OPEN (needs the Beekeeper's decision or a benchmark — do NOT settle unilaterally)

- **Fixed vs. temporal (age-polyethism) caste** — which builds a better hive for
  OSS needs. Founder leans temporal; must be benchmarked, not asserted. See
  north-star.md §14 for the proposed benchmark (throughput, tail latency under
  load spikes, recovery after a caste is knocked out, token cost).
- **Whether "drone" is used at all**, vs. keeping labor vocabulary clean.
- **The alignment beacon** — whether the queen-pheromone becomes a literal broadcast
  component in the AOS.

## 3. Integration tasks (pick up what fits today's work)

Ordered by leverage. Each is independently actionable.

1. **Propagate the lexicon & voice** into any Agix-facing copy you touch today —
   READMEs, site, product strings, agent/system prompts. Prefer hive vocabulary
   (colony/forage/comb/hive) over generic AI terms where tone allows. Keep
   Beekeeper ≠ Queen intact everywhere.
2. **Draft the first blog:** *"The comb remembers"* — stigmergy → shared-memory /
   coordination-through-artifacts. Highest brand leverage; grounds the "comb is
   both memory and coordination substrate" claim. Voice per §6. (Alt seeds in §11.)
3. **Visual identity starter:** produce a hexagon-based logo concept + an amber/
   comb-black palette token set (hex values, light/dark) a designer or build step
   can consume. Reference §6.
4. **Wire the philosophy into the AOS architecture** *(requires the AOS repo — not
   in `agix-ai/.github`; ask the Beekeeper to add it to scope first)*: align caste
   naming with §9, sketch the drone/guard inter-hive trust boundary (§12), and the
   optional alignment-beacon (§13).
5. **Set up the caste benchmark** (§14) if you have the AOS runtime — fixed vs.
   temporal on an identical workload; report the four metrics; let data decide.

## 4. Guardrails (do-nots)

- Do **not** frame the human as commanding a subordinate mind. Steward, not boss.
- Do **not** invent bee biology to fit a point — accuracy is the moat. Check facts.
- Do **not** drift to cold-blue / sterile-SaaS visuals; warmth is the differentiator.
- Do **not** open a PR or merge without the Beekeeper's explicit go-ahead.
- Do **not** resolve §2 open questions by fiat — surface them, propose, let the
  Beekeeper (or a benchmark) decide.
- On cross-hive/drone work: security is mandatory — authenticated, authorized,
  auditable. Never ship an open inter-hive channel.

## 5. Provenance

This came from a brand/philosophy ideation session between the Beekeeper (Brandon
Lewis / B Lewis Maker, Boulder CO) and the hive. `north-star.md` is a *living*
document — extend it as the philosophy sharpens; don't silently rewrite decided
sections. When you complete an integration task, note it back so the memory and the
product stay in sync.
