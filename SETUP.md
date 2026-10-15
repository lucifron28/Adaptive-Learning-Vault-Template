# Setup guide — choose your learning workflow

**No particular programming language, paid AI plan, editor, or operating system is required.** The vault is ordinary Markdown. This guide describes tested and optional workflows, not guaranteed account features.

## 1. Create your personal vault

1. Open the [Adaptive Learning Vault Template](https://github.com/lucifron28/Adaptive-Learning-Vault-Template).
2. If the **Use this template** button is available, select **Create a new repository**. Otherwise, download the files and create your own repository manually.
3. Choose **Private** if your notes will include personal assessments, project details, or mistakes you do not want public.
4. Read [Learning System/START HERE.md](Learning%20System/START%20HERE.md). Start with **one course** you actually want to study. Other topics can come later.
5. Optional: clone your new vault locally and open the folder in [Obsidian](https://obsidian.md/) as a vault. Markdown also works in VS Code or any text editor.

Template repositories create independent new repositories, unlike forks: [GitHub documentation](https://docs.github.com/en/repositories/creating-and-managing-repositories/creating-a-repository-from-a-template).

## 2. Choose a mode

| Mode | Good for | Can it run *your* code automatically? | Required setup |
| --- | --- | --- | --- |
| **ChatGPT in a web browser** | First-principles lessons, active recall, code explanations, interactive diagnostics | **Not by default.** Execution depends on tools, files, or runtime access in that conversation | AI chat; optionally connected GitHub |
| **Codex (local app / IDE / CLI)** | Real repository review, builds, tests, debugger-oriented tasks | **Often yes**, when the correct workspace and dependencies are accessible and permission permits | Coding environment, project checkout, Codex sign-in |
| **Codex cloud** | Delegated code review / tests in a configured cloud environment | **Potentially**, only with repository/environment access and installed dependencies | Codex cloud access, source access, environment configuration |
| **Other AI assistants or offline/manual** | Using the same teaching loop without ChatGPT | Depends on that assistant's tools | Copy/paste the mentor instructions and maintain Markdown manually |

**Author's currently tested experience (October 2026):** ChatGPT Plus, GPT-6 in regular ChatGPT web chat, with connected GitHub, has worked well for long, interactive teaching sessions. This is an experience report, **not a minimum requirement or a claim of unlimited messages**. Other plans/models and tools can follow the same learning process. ChatGPT and Codex have limits and feature availability that may change; check [GPT-6 model availability](https://help.openai.com/en/articles/20001354-gpt-6-and-other-models-in-chatgpt) and [Codex plan usage](https://help.openai.com/en/articles/11369540-using-codex-with-your-chatgpt-plan).

### Option A — ChatGPT on the web (simple, recommended starting point)

1. Sign in at [chatgpt.com](https://chatgpt.com/). A paid plan is **not required** for the basic copy-and-paste tutoring workflow.
2. Start a **new conversation** for a course. If you have access to model selection, GPT-6 is the author's tested choice; select a thinking setting as appropriate if available. Do not assume any model or plan has unlimited use.
3. Open [Reusable Software Engineering Mentor](Learning%20System/Reusable%20Software%20Engineering%20Mentor.md) and paste it into the conversation as the first message. For a new course, let the mentor ask for the subject, run a brief diagnostic, and create an adaptive roadmap.
4. **If your ChatGPT account offers a GitHub integration/plugin**, connect it from the available Plugins/apps settings, authorize *your own* repository and verify access by asking the assistant to read the README and your \`Learning Progress.md\`. A URL alone does not guarantee the assistant can read private repositories. Grant the smallest permissions you need.
5. If GitHub access is unavailable, **paste or upload** the relevant \`Learning Progress.md\` and current handoff (or small code snippets) in the chat. Save generated notes back into your vault manually. Do not assume edits or GitHub commits happened without confirmation.
6. Each time a lesson is **actually evaluated and completed**, have the mentor update the lesson note and progress record *if it has write access and you authorize it*, or supply copy-ready Markdown.
7. Continue using the exact next unfinished exercise in the progress file. For a new chat, use the continuation prompt below.

**Optional: ChatGPT Projects.** Create a Project for each learning track, add the short [ChatGPT Project Instructions](Learning%20System/ChatGPT%20Project%20Instructions.md) to **Project settings → Instructions**, and include your latest progress/handoff as project sources when helpful. Project instructions do not automatically keep GitHub files synchronized; use the connected integration or update files yourself. Don't paste two conflicting full mentor prompts into different instruction locations. [Official Projects guidance](https://help.openai.com/en/articles/10169521-projects-in-chatgpt).

### Option B — Codex for learning with executable verification

**Why use it:** Codex may inspect a checkout, run available commands and tests, and review diffs directly. It can provide stronger evidence than an AI chat that only sees snippets or learner-pasted output. **But tool access and a successful test run must still be verified; Codex is not automatically more pedagogically effective.**

1. Generate your own vault from the template, then **clone it** locally. Also clone your independent **application/project repository** if you have one.
2. Open the relevant folder in the Codex desktop app, Codex IDE extension, or Codex CLI and sign in with your ChatGPT account where supported. Choose the client and installation instructions from the current [Codex documentation](https://developers.openai.com/codex/cli) and [Codex with ChatGPT plans](https://help.openai.com/en/articles/11369540-using-codex-with-your-chatgpt-plan). Availability and permissions depend on your plan and environment.
3. This template includes an [AGENTS.md](AGENTS.md) teaching contract for agents that support repository instructions. Codex discovers \`AGENTS.md\` in its working directory hierarchy. **If Codex is opened in a separate application repository, the vault's AGENTS.md is not automatically applied there.** Paste the reusable mentor prompt into that session or add an appropriate \`AGENTS.md\` to your own project.
4. In the vault, request a **new-course diagnostic** or ask Codex to read your latest course progress and resume. When reviewing app code, give the app path/checkout and relevant commit. Confirm Codex can actually access them.
5. **Learning mode:** the learner writes the code first. Codex should review code, explain failures, run non-destructive builds/tests with appropriate permissions, and provide hints. It should **not** implement the assignment or alter application source by default.
6. After the learner's work is assessed, Codex may update the vault's Markdown files **when authorized**; inspect \`git diff\`, confirm evidence and avoid committing secrets. Have the learner decide when to push changes.
7. If a test cannot run (missing SDK, dependencies, network access, database, platform features), say exactly why. Fall back to source review plus learner-executed commands. Never invent test results.

**Optional hybrid workflow:** Use ChatGPT web for the teaching conversation and Codex for a targeted source review or test run. Paste the Codex findings, command output, and commit link back into the teaching chat; keep the same \`Learning Progress.md\` as the shared checkpoint. Avoid recording competing "master" progress in different chats.

### Option C — no integration, no Codex, no Obsidian

Use an ordinary AI chat with the mentor prompt. Copy your most recent progress and exercises into the conversation, run code in your own editor/terminal, paste error messages/results, and maintain Markdown files manually. The learning system still works.

## 3. Copy-ready first and returning messages

**Start a new course** (after providing the mentor instructions):

> I'm starting a software engineering learning track. Please ask what I want to study, diagnose my current conceptual and coding ability in short rounds, and build a staged curriculum with measurable checkpoints. Do not provide solutions before I attempt the exercises. I will choose the language and tools based on my goals.

**Resume an existing course:**

> Resume my course using the current \`Learning Progress.md\`, course handoff, and any relevant project files/commit. Treat the progress tracker as authoritative. Ask only the exact next unfinished exercise and one short recall check if due. Review my own implementation before suggesting fixes. Record only evaluated results; don't assume you can write to GitHub or run my code unless you verify access.

**Codex verification request:**

> Review my attempt at this task in the checked-out project without editing my application code. Inspect the relevant files/diff. Run only safe tests/builds when permitted. Report what you actually ran, the results, specific findings and focused hints. Distinguish source-only observations from runtime evidence. Wait for me to attempt corrections.

## 4. Normal study session

\`\`\`text
Read progress → spaced recall if due → one objective → learn
→ learner attempts → review actual evidence → fix/retest
→ record completed lesson → update review queue → resume later
\`\`\`

The learning record is more important than the chat history: it allows the same course to continue in another chat or agent. Keep one authoritative \`Learning Progress.md\` per course, avoid writing duplicate status snapshots, and do not mistake a long prompt or a large commit count for mastered skills.

## 5. Setup troubleshooting

| Symptom | What to do |
| --- | --- |
| AI cannot read a private repository | Verify authorization and repository access; otherwise paste/upload the needed files. |
| AI says it updated notes but GitHub hasn't changed | Inspect the repository/commit or \`git status\`; do not assume persistence. |
| Codex cannot run tests | Check the active workspace, runtime/SDK, test command, dependencies, database and permissions. Record limitation. |
| New chat repeats the diagnostic | Supply the current progress and handoff; explicitly say "resume the unfinished task." |
| Notes disagree across README/handoff/progress | Make \`Learning Progress.md\` authoritative. Use brief links from summaries. |
| Local Obsidian notes appear stale after remote commits | In the local vault run \`git status\`, resolve local changes safely, then \`git pull --ff-only\`. Don't overwrite work. |
| ChatGPT or Codex says usage has run out | Review the application's displayed plan usage/reset information; no unlimited use is promised. |

## Official references

- [OpenAI: GPT-6 models in ChatGPT](https://help.openai.com/en/articles/20001354-gpt-6-and-other-models-in-chatgpt)
- [OpenAI: Using Codex with your ChatGPT plan](https://help.openai.com/en/articles/11369540-using-codex-with-your-chatgpt-plan)
- [OpenAI: ChatGPT Projects](https://help.openai.com/en/articles/10169521-projects-in-chatgpt)
- [OpenAI: Codex CLI](https://developers.openai.com/codex/cli)
- [OpenAI: Agent instruction conventions](https://developers.openai.com/codex/guides/agents-md)
- [GitHub: Creating from a template](https://docs.github.com/en/repositories/creating-and-managing-repositories/creating-a-repository-from-a-template)
