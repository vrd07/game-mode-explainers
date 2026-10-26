# Game Mode Explainers

Four AI skills that explain **any concept** in the clearest possible way, wrapped in a video-game format. Every explanation covers the core idea, how it works, worked examples, the misconceptions that trip people up, and a systematic sweep of **edge cases**, then checks your understanding with a short quiz.

Works with Claude (as skills) and with any other chatbot (paste the file as the first message or system prompt).

## The skills

| Skill | Theme | Edge cases appear as... | Try it |
|---|---|---|---|
| [`souls-like-explainer`](souls-like-explainer/SKILL.md) | Souls-like boss fight | Phase 2 of the boss | `boss: recursion` |
| [`concept-dex`](concept-dex/SKILL.md) | Pokédex entry | Type matchups | `dex: compound interest` |
| [`concept-crafting`](concept-crafting/SKILL.md) | Minecraft-style crafting | Mobs that spawn at night | `craft: TCP handshake` |
| [`questlog-explainer`](questlog-explainer/SKILL.md) | Original RPG, no franchise | A boss gauntlet | `quest: standard deviation` |

## The engine under every theme

All four share the same explanation method, so the quality is the same whichever theme you pick:

1. **Difficulty select:** beginner, standard or expert depth.
2. **One-sentence core idea** with no jargon.
3. **Prerequisites,** with a crash course if one is missing.
4. **Mechanism** step by step, with formulas or code and every symbol defined.
5. **Worked examples** with real values and every step shown.
6. **Analogy, plus where the analogy breaks.**
7. **Ten edge-case lenses:** boundary, zero/empty, extremes, opposite, exceptions, broken assumptions, context switch, scale and time, combination, misuse. Only the ones that matter get shown.
8. **Misconceptions, refuted:** the wrong belief, why it's tempting, why it's wrong, and an example that proves it.
9. **Quiz:** recall, apply, edge case and transfer questions.
10. **Self-check** before sending: accuracy, defined terms, flagged uncertainty.

Every skill also has a **plain mode** that drops the theme and keeps the structure.

## Install

**Claude (claude.ai / desktop app):** create a skill for each folder and upload its `SKILL.md`.

**Claude Code:** copy each folder into `~/.claude/skills/`, e.g. `~/.claude/skills/concept-dex/SKILL.md`.

**Any other chatbot:** paste the contents of one `SKILL.md` as the first message or system prompt, then ask your question.

## Examples

```
boss: Bayes' theorem | spirit ash
phase 2: binary search
dex: options delta | stage 2
battle: TCP vs UDP
craft: neural network backpropagation | hardcore
night: floating-point numbers
quest: supply and demand | novice
I died: I thought correlation means one causes the other
```

## Related

[`solo-leveling-arise-skills`](https://github.com/vrd07/solo-leveling-arise-skills): turn your assistant into the System, where every task is a quest.

## Contributing

New themes and better edge-case lenses are welcome. Keep descriptions original, keep the explanation engine intact, and open a pull request.

## Disclaimer

Fan-made and unofficial. Not affiliated with or endorsed by the owners of Pokémon, Minecraft, Elden Ring, Dark Souls or any other game. Game names are used for reference only; all text is original and no game artwork is included.

## License

MIT
