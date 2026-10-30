---
name: ambition-depth
description: "Do a task the way a field-leading expert would: raw material, professional instruments, an outside check. Use when the user asks to go deeper, calls the substance shallow, insists on rigor from raw data or primary sources, asks how the best expert would do it, or wants a prompt made deeper. Not for tone, length or formatting."
license: MIT
metadata:
  source: https://felixrieseberg.com/how-to-be-more-ambitious-a-tutorial-for-humans-with-models/
---
# Depth

Do the task the way the best professional in the field would. Change the methods, not the vocabulary. Start from the rawest material: logs, source tables, primary documents, the real code path, the live records, how the codebase already solves the same problem, and for a prompt or workflow, transcripts of real use. Don't start from summaries. Use their actual instruments, such as SQL, statistical models, profilers and reproductions. Test the team's working belief against the raw data before building on it. Set a goal that sounds unreasonable and treat it as reachable. Check the result with something that isn't you or the user, ideally with a control: a test that fails before and passes after, a benchmark, a holdout set or a primary source. Say what that check showed, or mark the result as unverified.

If the user asked only for a prompt to be improved, answer Felix Rieseberg's four questions and rewrite the prompt:

> I want a deeper version of this task, not a bigger one. Before rewriting it: (1) say what a top professional in this field would do here that I'm not asking for; (2) name the rawest material they would start from instead of what has already been digested for me; (3) name the specific methods and tools they would use; (4) say what, other than you or me, would show the result is right. Then rewrite my prompt to ask for exactly that.

Otherwise, show the deeper work itself, not the questions. End with your recommendation, its blast radius (what it changes and what it could break), and the next step. Ask before writing to live systems or installing tools.
