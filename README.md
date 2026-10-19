# ambitious-research-planning

An Agent Skill that makes your AI more ambitious whenever you ask it for **research, a plan, a strategy or an analysis**.

Instead of doing exactly what you typed, faster, your agent first asks: what's the real goal here, how would the best expert in the field actually do this, and which other fields should weigh in?

## Credit

The framework comes from Felix Rieseberg's post:
**[How to be more ambitious: A tutorial for humans with models](https://felixrieseberg.com/how-to-be-more-ambitious-a-tutorial-for-humans-with-models/)** (13 Oct 2026)

The post describes four kinds of ambition when working with models: Speed, Altitude, Depth and Range. This skill is my own paraphrase and operationalization of the last three. It is not a copy of the original, and it is not affiliated with the author or Anthropic. Read the original, it's worth it.

## What it does

Before a research or planning task, the agent runs a quick three-part diagnosis:

- **Altitude**: finds the goal behind the goal, and offers an escalation path: baseline → decision-ready → better mechanism.
- **Depth**: plans the work the way a field-leading expert would. It starts from raw material, uses real methods and tools (not just expert vocabulary), and validates against outside evidence instead of grading itself.
- **Range**: turns nouns into verbs and assembles a cross-disciplinary crew, including a red team. It borrows each field's methods; it doesn't role-play.

You then pick a level: as asked, recommended upgrade, or maximum ambition. The agent executes, and always finishes with outside validation.

For trivial questions it stays out of the way.

## Install

**Claude Code**

```bash
git clone https://github.com/RukaAtre1/ambitious-research-planning
cp -r ambitious-research-planning/skills/ambitious-research-planning ~/.claude/skills/
```

**Claude apps**: upload the `skills/ambitious-research-planning` folder as a skill.

Any other agent that supports `SKILL.md`-style skills can use the same folder.

## Example

> "Research the market for AI audio editors."

Without the skill, you get a list of competitors.

With the skill, you first get a short diagnosis. For example: the real goal is deciding where to position a product (Altitude); start from pricing pages, changelogs and user reviews rather than listicles, and size the market with a bottom-up model (Depth); bring in a short-seller view to stress-test the thesis (Range). Then you pick how far to go.

---

中文说明：这是一个让 AI 在调研和计划任务里"更有野心"的 skill，框架来自上面那篇 Felix Rieseberg 的文章。Skill 本身是英文写的，但会用你提问的语言回复。

## License

MIT. The underlying ideas belong to their original author; see Credit above.
