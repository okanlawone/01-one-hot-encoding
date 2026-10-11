# Project 1: Build an inspectable one-hot encoder

Turn the unordered `department_name` category into clear 0/1 feature columns, then make the small preprocessing program easier to inspect and explain.

**Repository:** [okanlawone/01-one-hot-encoding](https://github.com/okanlawone/01-one-hot-encoding)  
**Course index:** [ai-engineering-journey](https://github.com/okanlawone/ai-engineering-journey)

## What you will learn

- Explain why department names are nominal categories with no natural numeric order.
- Trace how `pd.get_dummies()` makes one column per category and how `join()` attaches those columns by row index.
- Add simple checks so the output shape and one-flag-per-row assumption are visible.

## Project format

This is an open-ended, multi-session project. The starter program demonstrates the core idea; your work is to inspect it, extend it, and explain the choices. There is no one-day deadline. Pick up at the next unchecked item in [`progress.md`](progress.md). The detailed background and project brief are in [`lesson.md`](lesson.md).

## Checkpoints

- [ ] **Understand the baseline:** Run `main.py`; point out the source column, the new indicator columns, and the joined result.
- [ ] **Explore the category set:** Add one clearly invented department to a practice copy of the CSV and observe how the generated columns change.
- [ ] **Make the transformation reusable:** Refactor the transformation into a clearly named function that returns the combined DataFrame; keep the original category column.
- [ ] **Explain the assumptions:** Write down what happens if a category is missing or a new department appears, and why a future model may need a stable feature-column schema.

## Run the starter project

Clone this project repository, then run these commands from its root:

```bash
git clone https://github.com/okanlawone/01-one-hot-encoding.git
cd 01-one-hot-encoding
python3 -m venv .venv
source .venv/bin/activate
python -m pip install -r requirements.txt
python main.py
```

The code reads its CSV from the project folder, so it does not depend on your terminal’s current directory. The small CSV is invented practice data; it is not real customer data. See [`lesson.md`](lesson.md) for the data and training-data distinction.

## What counts as complete

Use the checklists in `lesson.md` and `progress.md`. A project is ready to close when the required behavior works, you can explain why the choices make sense, and the data limitations are documented. Optional extensions can wait for a later version.

**Optional extension:** Explore a missing department and an unseen department in separate practice copies. Describe the behavior before deciding how a production preprocessing pipeline should handle either case.
