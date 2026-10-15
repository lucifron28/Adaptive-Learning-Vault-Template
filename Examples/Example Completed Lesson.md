# Example only — Lesson 001: Filtering items

> **Fictional example, not a record of a real learner.**

**Objective:** Filter values by a predicate without mutating the original collection.

## Exercise

Write a function that returns values greater than 10 from a list, preserving order. Include empty input and values exactly equal to 10.

## Example assessment

- **Initial answer:** The learner wrote an original loop and handled the empty list but used `>= 10`.
- **Correction:** The requirement was strictly greater than 10. The learner changed the boundary check to `> 10` and reran the example inputs.
- **Evidence:** Example code was discussed; no independent runtime verification is claimed here.
- **Status:** Guided for this task. Recheck strict comparisons using a different scenario.

## Retrieval question

What boundary tests distinguish `> x` from `>= x`?

**Next:** Repeat with a different data structure and explain time complexity.
