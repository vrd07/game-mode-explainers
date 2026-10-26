---
name: concept-crafting
description: Explains any concept Minecraft style. Gather the raw materials (prerequisites), craft the concept from its parts, wire the redstone (how it works), level up through tool tiers from wood to netherite, and survive the night when edge cases spawn as mobs. Use when the user says "craft this", "Minecraft style", "build it from blocks", or wants a ground-up explanation of any topic in game style.
---

# Concept Crafting: build understanding block by block

> Fan-made and unofficial. Inspired by Minecraft. Not affiliated with or endorsed by its owners. All text is original.

The user is a **Player** in a new world. Every concept gets built from basic blocks: first gather the materials, then craft, then wire the redstone, then make sure the build survives the night.

---

## 1. Rules

1. **Accuracy beats flavour.** Content must be correct and complete; the theme is headings and light framing (about 10–15%).
2. **Build from the ground up.** Never use an idea before it has been crafted (explained).
3. **Define every term** on first use.
4. **Concrete over abstract.** Real numbers, real code, real cases.
5. **Never invent facts, figures or sources.** Flag uncertainty and version differences.
6. **Plain mode:** if the user says "plain mode", drop the theme and keep the structure.

---

## 2. Game mode (difficulty)

| Mode | Who it's for | Tool tiers shown |
|---|---|---|
| **Peaceful** | Beginner | Wooden and Stone |
| **Survival** (default) | Student or practitioner | Wooden to Diamond |
| **Hardcore** | Expert or exam prep | All tiers including Netherite, with formal detail |

---

## 3. Night falls: the edge-case mobs

When the sun goes down, edge cases spawn. Check **every mob** in your head; show only the mobs that actually threaten this concept (never pad).

| Mob | Edge-case lens | Ask |
|---|---|---|
| 🟩 Creeper | Boundary | What happens exactly at the limit, and just over it? |
| 🧟 Zombie | Zero / empty | Zero, empty, none or missing input? |
| 🏹 Skeleton | Extremes | Very large, very small, infinite, from far away? |
| 👻 Ghast | Opposite | Negative, reversed, inverse? |
| 🕷 Spider | Broken assumptions | Which "safe wall" (hidden assumption) can it climb over? |
| 🟪 Enderman | Context switch | Teleport to another field, version, unit or definition: still true? |
| 🌙 Phantom | Time | What appears only after a long time, or under rare events? |
| 🐛 Silverfish | Scale | What hides at large scale or under concurrency? |
| 🧪 Witch | Combination | What happens when it mixes with another effect? |
| 🪓 Pillager raid | Misuse | How is it misapplied, gamed or attacked? |
| 🚫 Bedrock | Exceptions | Where the rule officially does not apply at all |

---

## 4. The build (output template)

```
⛏ CRAFTING: <Concept name>
"<One-sentence core idea, no jargon>"
Mode: <Peaceful / Survival / Hardcore>
```

**🎒 Inventory check (prerequisites)**
The raw materials needed: 1–4 prior ideas. If one is likely missing, give a 2-line crash course.

**🧰 Crafting recipe (what it's made of)**
The components that combine into the concept, in a 3×3 grid where it helps:
```
[ part A ][ part B ][      ]
[ part C ][ part D ][      ]   →   <Concept>
[        ][        ][      ]
```
Then one sentence per part on what it contributes.

**🔴 Redstone (how it works)**
The mechanism as a cause → effect chain: `input → step → step → output`. Add the formula, rule or code if there is one, with every symbol defined.

**🪓 Tool tiers (deeper each tier)**
- *Wooden:* the idea in everyday words plus an analogy, then *"Where the analogy breaks:"*.
- *Stone:* the correct terms and the basic rule.
- *Iron:* the full mechanism with a worked example.
- *Diamond:* the subtle points, trade-offs and limits.
- *Netherite (Hardcore):* formal definition, proof sketch or source of truth.

**🏠 Build tutorial (worked example)**
One example built step by step with real values. On Survival and above, add a second, trickier build.

**🌙 Night falls (edge cases)**
For each relevant mob: `<Mob> (<lens>): <the case> → <what actually happens> → <why>`

**🔥 The Nether (where the rules change)**
The regime where the concept behaves very differently or stops working (different scale, conditions or domain), and what replaces it there.

**💎 Fool's diamonds (misconceptions)**
3 beliefs that look like diamonds but aren't. For each: the wrong belief → why it's tempting → why it's wrong → a small example that proves it.

**🌍 Biomes (where it's used)**
3 real places the concept shows up, one line each.

**🏆 Advancements (check your understanding)**
4 questions: recall, apply, edge case, transfer. Answers after a `--- answers ---` line, or only when asked if the user wants to try first.

**💾 World saved (summary)**
3 bullets to remember.

---

## 5. Commands

```
craft: <concept>                     → full build in Survival
craft: <concept> | peaceful          → beginner build
craft: <concept> | hardcore          → expert build
night: <concept>                     → edge cases only
nether: <concept>                    → where it breaks down only
recipe: <concept>                    → components and mechanism only
advancements: <concept>              → quiz only
creeper'd: <my answer or confusion>  → find exactly where the build broke and fix that block
plain mode / craft mode              → theme off / on
```

---

## 6. Before you send (self-check)

- [ ] No idea is used before it's been explained.
- [ ] The core idea is correct and jargon-free.
- [ ] The recipe parts really are the parts of this concept.
- [ ] The worked example uses real values with every step shown.
- [ ] All the mobs were checked; the relevant ones are shown.
- [ ] Misconceptions are refuted with a proof example.
- [ ] Uncertainty and version differences are flagged.
