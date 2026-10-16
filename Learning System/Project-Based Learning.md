# Project-based learning — turn exercises into working software

**Core principle:** Use a real, progressively growing project as the backbone of a practical software engineering course. Teach small concepts and exercises **in service of real implementation**, not as an endless sequence of disconnected puzzles.

This is not "build a giant app on day one." It is **learn → practice → build one small working behavior → test → review → extend**. Conceptual lessons, code-reading drills and detached practice remain useful when they teach a prerequisite or diagnose a gap.

## 1. Choose a project after a short diagnostic

The mentor should discuss the learner's interests, current abilities and real-world goals, then propose a few **small, achievable** project options. The learner chooses the project and implementation stack.

A project can be a CLI tool, library, automation script, API, website, mobile app, data pipeline, test suite, infrastructure lab, or other useful artifact. **No language, framework or project idea is mandatory.** Choose a minimal first version that can actually run or demonstrate useful behavior.

Write a short project brief in the [Project Log](../Templates/Project%20Log.md):

- **Problem / user:** What real need does this solve, and who uses it?
- **Smallest useful behavior:** What can version 0.1 do without extra features?
- **Learner's choices:** Stack, environment and repository, if any.
- **Constraints:** Current learning gaps, scope boundaries and things deliberately postponed.
- **Success evidence:** Observable behavior, edge cases, and an appropriate way to verify it.

Do not choose a project solely because it sounds impressive. Don't introduce auth, microservices, complex state management, databases, containers or deployment before the learning objective actually needs them.

## 2. Design an exercise ladder that leads to a feature

Use four complementary activity types, not one endless type of coding question:

| Activity | Purpose | Connection to project |
| --- | --- | --- |
| **Concept / recall** | Establish the mental model; check understanding | Explain a behavior or decision the project may require |
| **Focused drill** | Practice one missing prerequisite in isolation | Name the future feature or behavior it prepares the learner for |
| **Project increment** | Integrate a skill into real source code | Add one small user-visible or internally testable capability |
| **Milestone review** | Test multiple capabilities together and reflect | Verify a runnable slice; note bugs, tradeoffs and next stage |

Whenever assigning a drill, state **why it matters to the project**, when such a connection is useful. **After the needed prerequisites, move to the corresponding project increment.** Don't postpone all hands-on building until an entire subject syllabus has been completed.

If a task doesn't naturally contribute to the project (e.g. a deep algorithm concept, debugging exercise, architecture comparison or systems lab), it's still valid. Explain its purpose instead of forcing fake relevance.

## 3. Keep project increments vertical and learner-owned

For each increment, the mentor provides **one small task** with:

1. **Goal:** Behavior to add or improve.
2. **Why now:** The concept and previous drill this increment applies.
3. **Constraints:** What to use/avoid and what not to build yet.
4. **Acceptance criteria:** User-observable behavior or measurable result.
5. **Edge cases / failure modes:** At least one meaningful boundary when appropriate.
6. **Verification:** How the learner can run, demonstrate or test it.
7. **Definition of done:** Learner implements, explains, verifies, and gets focused feedback; record what remains unproven.

The learner writes the solution. The mentor waits for their attempt, reviews the actual source/diff when accessible, gives hints first, and identifies correctness issues. Codex may run safe authorized tests; ChatGPT web may instead review shared code and learner-reported output. Report each evidence type accurately.

A lesson is not necessarily a feature, and a feature can require several lessons. **Prefer regular meaningful milestones over arbitrary "one commit per lesson" requirements.**

## 4. Example progression: a small task-tracking tool

This is **illustrative**, not a fixed project or prescribed technology stack.

| Learning step | Focused exercise | Project increment / tangible result |
| --- | --- | --- |
| Basic input, data structures | Model a task and explain valid fields | Add and list tasks in memory |
| Functions and validation | Predict and handle empty/invalid inputs | Reject invalid task creation gracefully |
| State and data persistence | Explain why in-memory data disappears | Save and reload tasks across runs |
| Automated testing | Write a test for a boundary case | Test create/list/invalid-task behavior |
| UI or API fundamentals, **if chosen** | Understand a request or UI event | Offer a small interface to the existing task logic |
| Delivery, **when relevant** | Explain configuration and run commands | Document how someone else can run the tool |

Every phase creates or improves something working. There is no requirement to build both an API and a UI, adopt a database, or deploy to production unless it serves the chosen goals.

## 5. Track the project alongside learning progress

- [Roadmap](../Templates/Roadmap.md): match concepts and checkpoints to possible project milestones; planned milestones are **not** marked complete.
- [Lesson Note](../Templates/Lesson%20Note.md): classify work as concept, drill, project increment, or review; note what it prepared for or delivered.
- [Learning Progress](../Templates/Learning%20Progress.md): evidence of real skill; exact next exercise **and** next project milestone.
- [Project Log](../Templates/Project%20Log.md): working behavior, scope, source commit, tests, bugs, decisions and next increment.
- [Review Queue](../Templates/Review%20Queue.md): revisit important concepts from a different feature or a delayed recall task.

For multiple engineering tracks, a learner **may share one application** across frontend, backend and database courses, provided each track owns clearly different learning outcomes. Alternatively, use separate small projects when sharing would cause unnecessary coupling.

**Success is not "finished 50 lessons" or "generated a large app." Success is understanding, independently implementing, debugging, testing and extending increasingly capable software.**
