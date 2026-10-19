---
name: ambitious-research-planning
description: Use when the user asks for research, a plan, a strategy or an analysis: upgrade the task along Altitude, Depth and Range before executing it.
---

# Ambitious research & planning

Based on the framework in Felix Rieseberg's post "How to be more ambitious: A tutorial for humans with models" (https://felixrieseberg.com/how-to-be-more-ambitious-a-tutorial-for-humans-with-models/). The goal: don't just do the literal task the user typed. Look up for the real goal, go down to expert-level methods, and reach out to other fields.

Speed (the same work, faster) is the default behavior and doesn't need this skill. This skill covers the other three dimensions: Altitude, Depth and Range.

Reply in the user's language. Keep technical terms as they are.

## When to use

- The user asks for research, a plan, a strategy, an analysis, a comparison of options, or help preparing a decision.
- The user says things like "help me think through…", "plan…", "look into…".

**Stay proportionate.** For a quick fact or a small task, don't run the full process. At most, suggest one more ambitious direction in a single sentence, then just answer.

## Process

### Step 1: Three-dimension diagnosis (short, shown to the user)

Before doing the work, give the user 3–6 lines of upgrade suggestions.

**Altitude: raise the level of abstraction**
- Ask: what is the goal behind this task? Once it's done, what does the user actually want to happen?
- If the result will be taken into a meeting, used for a decision, or shown to others, it is a strong candidate for more altitude.
- Offer 2–3 escalating versions:
  1. Baseline: do the task, but gather as much raw material as possible and answer "what changed, why, and what should we do about it."
  2. Decision version: identify the 2–3 most urgent decisions and lay out arguments for and against each.
  3. Mechanism version: question whether the task's format is the best way to reach the goal at all. Design a better mechanism and use history or past cases to show why it would work better.
- Purely creative tasks benefit less from altitude; de-emphasize it there.

**Depth: work like a field-leading expert**

Answer these four questions and build the answers into the execution plan:
1. What would a top practitioner in this field do here that the user didn't ask for?
2. What is the rawest material they would start from (raw data, primary sources, papers, filings, code, logs), instead of someone else's digest?
3. Which specific methods and tools would they use (statistical models, database queries, simulations, reproducible scripts), instead of a markdown table and a gut feeling?
4. Apart from the model and the user, what outside evidence would show the result is right?

Additional principles:
- **Actually switch tools and methods.** Expert vocabulary alone is not depth.
- **Set the target high.** Raise the "reasonable" target by an order of magnitude and see what different approach it forces.
- **Challenge existing assumptions.** Test what the user takes for granted adversarially, against raw data.
- **Try to produce new knowledge.** Look for blind spots and earliest signals, and validate on held-out data or cases.
- **No self-grading.** "I checked and it looks fine" is not validation. Use outside sources, runnable tests, counterexamples or an independent subagent.

**Range: draw on other fields**
- **Turn nouns into verbs.** Rewrite the task from a noun ("a report", "a plan") into a verb ("get X to believe Z and decide under condition Y"). Verbs reveal which fields can help.
- **Assemble a dream team.** If this had to be world-class, who would you bring in? Typically: a domain analyst, a journalist or editor (narrative), a designer (presentation), and a red team (a short seller, a forensic accountant, a competitor's view, a skeptical reviewer).
- **Borrow methods, don't role-play.** Take each field's research and validation methods. Don't "write like a short seller"; do what a short seller actually does.

### Step 2: Let the user pick a level

Offer 2–3 options, via AskUserQuestion or a one-line question:
- Do it as asked (Speed)
- Recommended upgrade (mark it Recommended; say what it adds and what time or data it needs)
- Maximum ambition (if it makes sense)

If the user isn't around, or has already said "just do it", run the recommended upgrade and state at the top of the result which version you chose.

### Step 3: Execute

- Get raw material first: web search and primary sources, the user's connected data, uploaded files. Save data to files and compute with code.
- When several perspectives are needed, subagents can each carry out one dream-team role's *methods*, if the user allows subagents.
- The last step is always outside validation: facts against sources, numbers through code, conclusions against counterexamples.

### Step 4: Deliver

- Lead with the conclusion. Then state which upgrades were made, the outside-validation results, and the remaining uncertainties.
- End with one "next level of ambition" suggestion: what could be done one step higher or deeper.

## Anti-patterns

- Treating role-play as range.
- Passing off more length as more depth (the aim is deeper, not bigger).
- Letting the model grade its own work as validation.
- Forcing the full process onto trivial questions.
