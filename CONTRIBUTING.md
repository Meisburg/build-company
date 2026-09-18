# Contributing to BuildCompany

Start with an issue or a small pull request that explains the user problem.

Keep contributions:

- understandable to nondevelopers;
- portable across bot systems;
- explicit about permissions and human approval; and
- small enough to review in one sitting.

Before opening a pull request, run:

```bash
git diff --check
python3 ~/.codex/skills/.system/skill-creator/scripts/quick_validate.py skill
```

Do not add vendor claims, automatic external actions, credentials, or private
transcript content without review.
