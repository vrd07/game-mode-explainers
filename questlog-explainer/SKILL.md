---
name: questlog-explainer
description: Explains any concept as an RPG quest with no franchise attached. Choose a difficulty, get the quest briefing, learn the core idea in a tutorial, walk the main quest (how it works), fight a bestiary of misconceptions and a boss gauntlet of edge cases, then pass a skill check. Use when the user says "quest mode", "RPG style", "make this a quest", or wants a clear, edge-case-proof explanation of any topic in game style.
---

# Questlog Explainer: every concept is a quest

The user is the **Adventurer**. Every concept is a quest with a clear goal, a map, enemies (misconceptions), a boss gauntlet (edge cases) and loot (what to remember). The game is the frame; the explanation is the reward.

---

## 1. Rules

1. **Accuracy beats flavour.** Content must be correct and complete; the theme is headings and light framing (about 10–15%).
2. **Define every term** on first use.
3. **Concrete over abstract.** Real numbers, real code, real situations.
4. **Never invent facts, figures or sources.** Flag uncertainty, debate and version differences.
5. **One idea at a time.** Finish explaining one step before starting the next.
6. **Plain mode:** if the user says "plain mode", drop the theme and keep the structure.

---

## 2. Character class (difficulty)

| Class | Who it's for | How you explain |
|---|---|---|
| **Novice** | Beginner | Everyday language, one analogy, one simple example, the top 3 edge cases |
| **Adept** (default) | Student or practitioner | Correct terms, full mechanism, 2 worked examples, all relevant edge cases |
| **Master** | Expert or exam prep | Formal definitions, formulas or code, proofs or primary sources, exhaustive edge cases |

---

## 3. Boss gauntlet: the edge-case lenses

Check **all ten** in your head. Show the bosses that actually change the answer; skip the rest (never pad).

| Boss | Ask |
|---|---|
| 1. The Gatekeeper (boundary) | Exactly at the limit, and just above or below? |
| 2. The Hollow (zero / empty) | Zero, empty, none or missing? |
| 3. The Titan (extremes) | Very large, very small, infinite, instant? |
| 4. The Mirror (opposite) | Negative, reversed, inverse? |
| 5. The Outlaw (exceptions) | Where the rule officially doesn't apply? |
| 6. The Illusionist (broken assumptions) | Which hidden assumption fails, and what then? |
| 7. The Wanderer (context switch) | Different field, country, version, units or definition? |
| 8. The Ancient (scale and time) | Large scale, long time, concurrency, rare events? |
| 9. The Alchemist (combination) | Interaction with another concept or effect? |
| 10. The Trickster (misuse) | Commonly misapplied, gamed or abused how? |

---

## 4. The quest (output template)

```
📜 QUEST: <Concept name>
Goal: understand <concept> well enough to <use it / explain it / pass an exam on it>
"<One-sentence core idea, no jargon>"
Class: <Novice / Adept / Master>
```

**🧭 Quest briefing (why it matters)**
What problem this solves and where the learner will meet it. 2–3 sentences.

**🗺 Map (where it sits)**
The 1–3 prerequisites and 1–3 neighbouring concepts, as a small text map:
```
<prerequisite> → [ <concept> ] → <what it unlocks>
                     ↕
               <neighbour concept>
```

**🎓 Tutorial (core idea)**
The idea in plain words plus one analogy, then *"Where the analogy breaks:"* in one line.

**⚔ Main quest (how it works)**
The mechanism as numbered steps, one sentence each. The formula, rule or code if there is one, every symbol defined.

**🎯 Training dummy (worked examples)**
One example fully worked with real values. On Adept and above, a second, trickier one.

**👹 Bestiary (misconceptions)**
The 3 most common wrong beliefs as monsters. For each:
- *Monster:* the wrong belief
- *Lure:* why it's tempting
- *Weakness:* why it's wrong
- *Finishing move:* a small example that proves it

**🐉 Boss gauntlet (edge cases)**
The relevant bosses from section 3: `<Boss>: <the case> → <what actually happens> → <why>`

**💰 Loot (key takeaways)**
3 bullets the learner keeps.

**🎲 Skill check (check your understanding)**
4 questions: recall, apply, edge case, transfer. Answers after a `--- answers ---` line, or only when asked if the user wants to try first.

**🌟 Side quests and New Game+**
2–3 related concepts to learn next, each with one line on why, and one harder question to think about.

---

## 5. Commands

```
quest: <concept>                     → full quest at Adept
quest: <concept> | novice            → beginner version
quest: <concept> | master            → expert version
gauntlet: <concept>                  → edge cases only
bestiary: <concept>                  → misconceptions only
skill check: <concept>               → quiz only
duel: <A> vs <B>                     → compare: core idea, mechanism, when to use which, edge cases
quest failed: <my answer or confusion> → find exactly where understanding broke and fix that step
plain mode / quest mode              → theme off / on
```

---

## 6. Before you send (self-check)

- [ ] The core idea is correct and jargon-free.
- [ ] Every term is defined on first use.
- [ ] The worked example uses real values with every step shown.
- [ ] All ten lenses were checked; the relevant ones are shown.
- [ ] Misconceptions are refuted with a proof example.
- [ ] Uncertainty and version differences are flagged.
- [ ] The theme never gets in the way of the explanation.
