# Adaptive Learning Vault — Software Engineering

**Learn software engineering with an AI mentor—without outsourcing your thinking.**

A **language-agnostic, evidence-driven learning system** built with plain Markdown. Study programming, frontend, backend, databases, algorithms, architecture, testing, security, or DevOps in **your chosen language and stack**.

> **Learning loop:** Diagnose → Learn → Attempt → Review → Correct → Apply → Recall → Record.

**Start here:** [Full setup guide](SETUP.md) · [Mentor prompt](Learning%20System/Reusable%20Software%20Engineering%20Mentor.md) · [Course workflow](Learning%20System/START%20HERE.md)

## Get started in 3 steps

1. Click **Use this template → Create a new repository** (when enabled by the owner). Make **your own vault private** if you will store personal learning records, project details or private links. Otherwise download/clone the files.
2. Choose a learning mode below. For the simplest path, copy the [mentor prompt](Learning%20System/Reusable%20Software%20Engineering%20Mentor.md) into a new AI chat.
3. Tell the mentor what area of software engineering you want to learn. Start with a **short diagnostic**, build an adaptive roadmap, and attempt exercises yourself. Only evaluated work is recorded as completed.

**No purchase, Obsidian installation, GitHub connector, or coding agent is required** for the basic copy-and-paste learning workflow. GitHub and Obsidian make the notes easier to persist and navigate, but Markdown files remain portable.

## Recommended learning setups

| | **ChatGPT web (easiest)** | **Codex (code verification)** |
| --- | --- | --- |
| Best for | Concepts, interactive mentoring, explanations, diagnostics, retention | Reviewing actual repositories and diffs; running available builds/tests |
| How it starts | Paste the mentor prompt into a chat, or use a ChatGPT Project | Open your checkout in a supported Codex client and use the included \`AGENTS.md\` / mentor prompt |
| What it can verify | Reasoning and provided code; repo inspection when connected | Source and runtime behavior when access, dependencies and permissions allow |
| Limitation | Cannot assume access to local files or running programs | Can over-solve assignments if not kept in learner-first mode |
| Required? | No | No |

**Author's tested setup (October 2026):** **GPT-6 in regular ChatGPT web chat with a ChatGPT Plus plan**, optionally with connected GitHub, works well for the long, interactive learning sessions that inspired this template. **Codex is a useful optional upgrade for testing/reviewing real code**, not necessarily a better tutor. The educational method also works with other models or assistants.

**Usage note:** The author has experienced long chat sessions, but **Plus is not guaranteed unlimited**. Model, feature, and Codex limits can vary over time. See [OpenAI's model guidance](https://help.openai.com/en/articles/20001354-gpt-6-and-other-models-in-chatgpt) and [Codex plan guidance](https://help.openai.com/en/articles/11369540-using-codex-with-your-chatgpt-plan). Verify available models and limits in your own account.

**Detailed walkthroughs:** [ChatGPT web setup](SETUP.md#option-a--chatgpt-on-the-web-simple-recommended-starting-point) · [Codex setup](SETUP.md#option-b--codex-for-learning-with-executable-verification) · [manual/other AI](SETUP.md#option-c--no-integration-no-codex-no-obsidian)

## What makes this different?

- **Adaptive diagnostics** rather than forcing every learner through the same beginner path.
- **One focused exercise at a time** with the learner's own attempt before any solution.
- Coding, reasoning, debugging, tests, and design tradeoffs assessed independently.
- **Recognized → Guided → Independent → Retained** evidence levels; no automatic mastery from exposure.
- A **small evolving project** rather than a large AI-generated scaffold.
- Review of *actual* repository changes when available, with honest distinctions among source review, learner-run output, and independently executed tests.
- Spaced recall and transparent documentation of mistakes, corrections and subsequent progress.
- Durable files that can be reused across ChatGPT chats, Codex, and other capable tools.

## What can I study?

Choose only what matches your interests, current skill level and learning goal—**these are examples, not a prescribed curriculum**.

| Area | Example concepts |
| --- | --- |
| Programming foundations | Types, collections, functions, debugging, complexity |
| Problem solving | Data structures, algorithms, edge cases |
| Software design | OOP, modularity, refactoring, architecture decisions |
| Frontend | Web fundamentals, JavaScript/TypeScript, UI frameworks, accessibility |
| Backend and APIs | HTTP, validation, concurrency, authentication, reliability |
| Data and storage | SQL, data modeling, constraints, indexes, transactions |
| Quality and security | Automated testing, code review, threat modeling |
| Delivery and operations | Git, CI, containers, observability, deployment |

Possible implementations include Python, C#, Java, JavaScript, TypeScript, Go, Rust, C++, PHP, and other languages. **No language is hardcoded into the system.**

## Repository layout

\`\`\`text
README.md                  One-minute overview and recommended paths
SETUP.md                   Full setup: ChatGPT web, Codex, manual workflow
AGENTS.md                  Short coding-agent learning rules
Learning System/           Mentor prompt, progress rules, workflow, Project instructions
Courses/                   Add your own courses; no fake completed lessons
Templates/                 Roadmap, lesson, progress, handoff, review and project log
Examples/                  Clearly fictional assessed lesson example
References/                Related projects and documentation
\`\`\`

Read [Start Here](Learning%20System/START%20HERE.md) and the [Assessment Rubric](Learning%20System/Assessment%20Rubric.md) to understand what earns completion. New chats should resume from the course's **current Learning Progress** file.

## How learning and verification coexist

**Chat mode:** discuss a concept → attempt a solution → receive corrective feedback → run code yourself when needed → share evidence → save an evaluated note.

**Codex mode:** inspect *your* attempt → execute non-destructive checks when available → report failures and give hints → **you correct the code** → record evidence. It should not write an exercise solution unless you ask explicitly. The root [AGENTS.md](AGENTS.md) sets that behavior for coding agents that load repository instructions.

You can also combine modes: use regular ChatGPT for mentoring and Codex for targeted verification, sharing reviewed commit links and test output back to your course's one authoritative progress file.

## Related projects and source inspiration

The [comparison notes](References/Comparable%20Projects.md) cover TutorVault, agent-tutor, Personal AI Teacher, LessonLab, and the official product documentation that informed the setup.

## Rules and privacy

- A **roadmap is a plan**, not evidence of actual learning.
- The learner owns assignments and chooses when source code may be changed.
- Never claim commands ran, tests passed, or files were committed without verification.
- Protect private reflections, tokens, personal information and private project links. Consider using a private generated repository even though this public template is shareable.
- ChatGPT and Codex integrations depend on account access and approvals; **Markdown itself does not perform background syncing**.

## Contributing and license

Improvements are welcome; read [CONTRIBUTING.md](CONTRIBUTING.md). Licensed under [MIT](LICENSE).
