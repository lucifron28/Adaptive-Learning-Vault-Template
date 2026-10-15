# Start here — Software Engineering Learning Vault

This is a reusable, language-independent learning system designed to develop real software engineering ability through assessment, practice, code review and recall—not passive tutorial completion.

**New user?** Read [SETUP.md](../SETUP.md) first to choose ChatGPT web, Codex, or a completely manual workflow. The system works with normal Markdown; Obsidian and GitHub connections are optional.

## First use

1. Create your own copy of this repository (prefer a private repository if saving personal assessments).
2. Choose an AI assistant and provide [the reusable mentor prompt](Reusable%20Software%20Engineering%20Mentor.md). Codex users should also note [AGENTS.md](../AGENTS.md); ChatGPT Projects users can use the [short Project Instructions](ChatGPT%20Project%20Instructions.md).
3. Choose an area of software engineering and explain a practical learning goal. The mentor should ask briefly about your experience and perform a short, interactive diagnostic.
4. Copy [Course Handoff](../Templates/Course%20Handoff.md), [Roadmap](../Templates/Roadmap.md), [Learning Progress](../Templates/Learning%20Progress.md) and [Review Queue](../Templates/Review%20Queue.md) into a course folder under `Courses/`. Adapt them to your selected stack, not to a default C# or JavaScript syllabus.
5. If relevant, choose one small cumulative learner-owned coding project after diagnosing prerequisites. Keep source code in a separate repository when useful.
6. Work through one interactive objective at a time. Attempt the task yourself. Save an evaluated [lesson note](../Templates/Lesson%20Note.md) and update progress **only after an actual assessment**.

## Everyday session

```text
Read Learning Progress → short spaced recall → one new objective
→ learner attempts → tutor reviews → correct/retest
→ record evidence and outstanding questions → next session
```

**Do not rely on a long chat alone for continuity.** Keep the latest checkpoint in a versioned file and use it across sessions and tools.

## Returning to a course in a new chat or agent

Supply the current `Learning Progress.md`, course handoff and, when relevant, the project repository/commit.

> Resume this course from its current Learning Progress. Don't redo the diagnostic or treat planned topics as completed. Ask the exact next unfinished exercise and review my attempt. Only claim running tests, inspecting source or saving files when those actions really occurred.

If GitHub/Obsidian access is unavailable, paste or upload the needed notes and save updated Markdown manually.

## Source of truth

- **Learning Progress.md** — latest assessed skills, exact unfinished task and evidence boundary.
- **Roadmap.md** — a flexible plan, not a completed checklist.
- **Lessons/** — actual evaluated lesson notes, not automatically generated transcripts.
- **Review Queue.md** — later retrieval tasks and gaps.
- **Project Log.md** — repository links, source reviewed, testing scope and decisions.

**Safety and ownership:** learner writes code by default. Connected agents may inspect and test when permitted; application modifications and Git pushes require user authorization. Changes to the learning vault should also be requested or approved. Avoid falsely claiming automatic synchronization or persistent memory.
