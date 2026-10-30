# Skills

Agent skills I use in my own work and share publicly. Each one is a single `SKILL.md` that follows the [Agent Skills spec](https://agentskills.io/specification), so it works with Claude Code, Codex, Cursor and other agents that support skills.

## Install

```bash
npx skills add Winston-Hsiao/skills
```

Pick one skill with `--skill <name>`, or add `-g` to install globally. See the [`skills` CLI](https://github.com/vercel-labs/skills) for all options.

## Ambition skills

Three skills based on Felix Rieseberg's [How to be more ambitious: A tutorial for humans with models](https://felixrieseberg.com/how-to-be-more-ambitious-a-tutorial-for-humans-with-models/). Each one covers one kind of ambition from the post. The post's fourth kind, Speed, is left out. Felix skips it too, calling it well established and the bread and butter of how people already use models.

| Skill | What it does | Reach for it when |
|---|---|---|
| [`ambition-altitude`](skills/ambition-altitude/SKILL.md) | Raises the task to the outcome it serves, the goal behind the goal, and works at that level. | You're handing over tasks one at a time, or the work feeds a decision, a recurring process or a meeting. |
| [`ambition-depth`](skills/ambition-depth/SKILL.md) | Does the task the way a field-leading expert would: starts from raw material, uses professional instruments, checks the result against something outside the model, and ends with a recommendation, its blast radius and the next step. | The answer matters and a plausible one isn't enough: reviews, root causes, analyses, "is this safe?" |
| [`ambition-range`](skills/ambition-range/SKILL.md) | Brings in methods from fields outside the obvious one, including a red team, and actually runs them. | You want other perspectives, a red team or a battle test, or the work feels conventional. |

Invoke one by name (in Claude Code, for example, `/ambition-depth`). They are also written so an agent can pick them up from phrases like "go deeper" or "what is this really for?".

They're short on purpose. Early versions spelled each technique out as numbered steps. In blind comparisons the agent then printed the procedure (ladders, crew tables, the four questions) instead of doing better work, and lost to no skill at all. The current versions say how to think and leave the output to the task.

I tested them in about four days of my own daily engineering work. `ambition-depth` changed the result most often. Its largest wins came from testing the team's working belief against the raw data, and from outside checks that had a control: a test that fails before the fix and passes after.

Know before using them:

- **Depth makes answers longer.** It may give an explanation request a decision memo. Ask for brevity, or cut the answer down as a separate step.
- **Range does real work.** It runs the other fields' methods, so expect it to cost more and take longer than a brainstorm.

## Credits

- The Altitude, Depth and Range framing and techniques come from [Felix Rieseberg's post](https://felixrieseberg.com/how-to-be-more-ambitious-a-tutorial-for-humans-with-models/). The prompt quoted in `ambition-depth` is his, word for word.
- Restating the deliverable in verbs instead of nouns, in `ambition-range`, is Felix's "replace the nouns with verbs" technique, which he credits to Tom Kelley and Jonathan Littman's *The Art of Innovation*.

## License

[MIT](LICENSE). The license covers my own text. The quoted prompt and referenced ideas belong to their authors.
