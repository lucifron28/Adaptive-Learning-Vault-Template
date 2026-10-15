# Related projects and documentation inspiration

This repository is a **language-independent software engineering learning template**. It draws general onboarding and instruction-design lessons from other open-source AI tutoring systems; it is not a fork of or affiliated with the projects below.

| Project | Published idea worth learning from | How this template differs |
| --- | --- | --- |
| [TutorVault](https://github.com/RobertttBS/TutorVault) | Obsidian-oriented onboarding, persistent syllabi, and agent-specific instructions | Focuses on software engineering, reviewed code, and verification evidence |
| [agent-tutor](https://github.com/Mohamed-El-Sharqawy/agent-tutor) | A portable agent learning workflow with vault notes and spaced repetition | Offers both regular ChatGPT web and coding-agent setup paths without requiring agent installation |
| [Personal AI Teacher](https://github.com/Uxielo/personal-ai-teacher) | Treats learner evidence, assessment and durable history as central to education | Uses simple Markdown templates and human-reviewed progress instead of imposing a separate grading CLI |
| [LessonLab](https://github.com/goneil78-coder/LessonLab) | Clear different setup paths for different AI products and users | Specifically mentors learners in software engineering rather than generating lesson plans for teachers |

## Practical principles adopted

1. Put the **one-minute setup** in the main README; keep platform-specific detail in [SETUP.md](../SETUP.md).
2. Make software-engineering pedagogy independent of ChatGPT/Codex product names.
3. Include both **chat-first** and **code-verification** workflows, with tool-access boundaries.
4. Put durable progress in Markdown so a new model, session, or tool can resume the same course.
5. Keep coding-agent instructions in a short \`AGENTS.md\`; don't force a huge checklist before every tiny task.
6. Do not call any tool or plan unlimited, and don't assume an agent can execute code just because it can review it.

## Product references (October 2026)

- [OpenAI: GPT-6 models and ChatGPT limits](https://help.openai.com/en/articles/20001354-gpt-6-and-other-models-in-chatgpt)
- [OpenAI: Codex plan availability and usage](https://help.openai.com/en/articles/11369540-using-codex-with-your-chatgpt-plan)
- [OpenAI: ChatGPT Projects](https://help.openai.com/en/articles/10169521-projects-in-chatgpt)
- [OpenAI: Rethinking instructions for GPT-6 Astra](https://developers.openai.com/blog/rethinking-skills-and-prompts-for-gpt-6-astra)
- [GitHub: Creating a repository from a template](https://docs.github.com/en/repositories/creating-and-managing-repositories/creating-a-repository-from-a-template)
