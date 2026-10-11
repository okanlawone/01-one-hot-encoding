# Project 1: Build an inspectable one-hot encoder — progress

**Guide status:** The starter files and project brief are published. Learner work on the open-ended checkpoints has not been verified, so the learning checklist starts unchecked.

Use this page across sessions. Check an item only after you have done it and can explain what you learned. If a step takes more than one sitting, leave it unchecked and write your next small move in the session log.

## Checkpoints

- [ ] **Understand the baseline:** Run `main.py`; point out the source column, the new indicator columns, and the joined result.
- [ ] **Explore the category set:** Add one clearly invented department to a practice copy of the CSV and observe how the generated columns change.
- [ ] **Make the transformation reusable:** Refactor the transformation into a clearly named function that returns the combined DataFrame; keep the original category column.
- [ ] **Explain the assumptions:** Write down what happens if a category is missing or a new department appears, and why a future model may need a stable feature-column schema.

## Completion criteria

- [ ] `main.py` reads the bundled CSV using a path relative to the script.
- [ ] Each observed department has a visibly named `dept_...` indicator column.
- [ ] The original review and department columns remain available in the result.
- [ ] For the current no-missing-value practice data, each row has exactly one department flag set to 1.
- [ ] Your explanation labels the CSV as invented practice data and does not call it model-training data.

## Session notes

Add one short entry whenever you stop. Keep your own observations here; blank entries are prompts, not claims about work already completed.

### Session 1
- Date:
- Checkpoint worked on:
- What I observed or changed:
- Question to resolve:
- Next small step:

### Session 2
- Date:
- Checkpoint worked on:
- What I observed or changed:
- Question to resolve:
- Next small step:

### Session 3
- Date:
- Checkpoint worked on:
- What I observed or changed:
- Question to resolve:
- Next small step:

### Later sessions
Add another heading when you need one.

## Optional extension

Explore a missing department and an unseen department in separate practice copies. Describe the behavior before deciding how a production preprocessing pipeline should handle either case.
