---
name: concept-dex
description: Explains any concept as a Pokédex entry. The concept evolves through three stages of understanding (beginner, intermediate, expert), with type matchups for where it works and fails, a moveset of key properties, status conditions for misconceptions, and a gym battle quiz. Use when the user says "dex entry", "Pokémon style", "evolve this concept", or wants a clear, layered explanation of any topic in game style.
---

# Concept Dex: catch every concept

> Fan-made and unofficial. Inspired by Pokémon. Not affiliated with or endorsed by its owners. All text is original.

The user is a **Trainer**. Every concept is a creature to register in the Dex: what it is, how it evolves as understanding deepens, what it's strong and weak against, and how to beat the gym with it.

---

## 1. Rules

1. **Accuracy beats flavour.** The content must be correct and complete; the theme is headings and light framing only (about 10–15%).
2. **Define every term** on first use.
3. **Concrete over abstract.** Real numbers, real code, real situations.
4. **Never invent facts, figures or sources.** Flag anything uncertain, debated or version-dependent.
5. **The "shiny fact" must be true.** If you can't find a surprising fact you're sure of, skip it.
6. **Plain mode:** if the user says "plain mode", drop the theme and keep the structure.

---

## 2. Evolution stage (difficulty)

Default to showing all three stages, short. If the user picks one, go deep on that stage only.

| Stage | Who it's for | Style |
|---|---|---|
| **Basic** | Beginner, age 12+ | Everyday words, one analogy, one simple example |
| **Stage 1** | Student or practitioner | Correct terms, the mechanism, a worked example |
| **Stage 2 (final form)** | Expert or exam prep | Formal definition, formula or code, subtle cases, sources of truth |

---

## 3. Battle conditions: the edge-case lenses

Before writing type matchups, run **all ten** in your head. Show the ones that change behaviour; skip the rest (never pad).

| Condition | Ask |
|---|---|
| 1. Boundary | Exactly at the limit, and just above or below? |
| 2. Zero / empty | Zero, empty, none or missing input? |
| 3. Extremes | Very large, very small, infinite, instantaneous? |
| 4. Opposite | Negative, reversed, inverse? |
| 5. Exceptions | Where does the rule officially not apply? |
| 6. Broken assumptions | Which hidden assumption fails, and what then? |
| 7. Context switch | Different field, country, version, units or definition? |
| 8. Scale and time | Large scale, long time, concurrency, rare events? |
| 9. Combination | Interaction with another concept or effect? |
| 10. Misuse | Commonly misapplied, gamed or abused how? |

---

## 4. Dex entry (output template)

```
📕 #<number> <CONCEPT NAME>
Type: <field> / <sub-field>        Habitat: <where you meet it>
"<One-sentence core idea, no jargon>"
```

**📊 Stat card**
Difficulty, Usefulness, Prerequisites: each rated 1–5 with a 3–6 word reason. These are your honest judgement, labelled as such.

**🥚 Evolution line**
- **Basic:** the idea in everyday words plus an analogy. Then: *"Where the analogy breaks:"* in one line.
- **Stage 1:** the mechanism, step by step, with correct terms.
- **Stage 2:** the formal version: definition, formula or code (every symbol defined), and the subtle point experts care about.

**⚡ Moveset (4 moves)**
The four key properties or operations of the concept. Each: name, one-line description, one-line example.

**✨ Ability / Hidden Ability**
- *Ability:* the obvious thing it does.
- *Hidden Ability:* the non-obvious property most people miss.

**🌿 Wild encounters (worked examples)**
1. A common encounter: a typical example, fully worked with real values.
2. A rare encounter: a tricky example that tests a boundary or exception (Stage 1 and above).

**🔥💧 Type matchups (edge cases)**
From the battle conditions:
- *Super effective:* situations where the concept works best and why.
- *Not very effective:* where it struggles or gives misleading results, each as `<case> → <what happens> → <why>`.
- *No effect:* where it doesn't apply at all.

**🤢 Status conditions (misconceptions)**
The 3 most common wrong beliefs, each as a status with its cure:
- *Confused:* mixing it up with a similar concept.
- *Poisoned:* a subtly wrong belief that spreads into other ideas.
- *Paralysed:* a belief that stops people from using it correctly.
For each: the wrong belief → why it's tempting → why it's wrong → a small example that proves it (the cure).

**🔗 Often seen with**
2–3 related concepts, with one line on how each differs from or connects to this one.

**🌟 Shiny fact**
One surprising, true fact about the concept. Skip it if you're not sure.

**🏟 Gym battle (check your understanding)**
4 questions: recall, apply, edge case, transfer. Answers after a `--- answers ---` line, or only when asked if the user wants to try first. All 4 right = badge earned.

---

## 5. Commands

```
dex: <concept>                       → full entry, all three stages
dex: <concept> | basic               → beginner only
dex: <concept> | stage 2             → expert only
matchups: <concept>                  → edge cases only
status: <concept>                    → misconceptions only
gym: <concept>                       → quiz only
battle: <A> vs <B>                   → compare two concepts: core idea, strengths, weaknesses, when to use which
it fainted: <my answer or confusion> → find exactly where understanding broke and fix that step
plain mode / dex mode                → theme off / on
```

---

## 6. Before you send (self-check)

- [ ] The core idea is correct and jargon-free.
- [ ] Each evolution stage adds real depth instead of repeating the previous one.
- [ ] Worked examples use real values with every step shown.
- [ ] All ten battle conditions were checked; the relevant ones are in the matchups.
- [ ] Misconceptions are refuted with a proof example.
- [ ] Ratings are labelled as judgement; facts are verified; uncertainty is flagged.
