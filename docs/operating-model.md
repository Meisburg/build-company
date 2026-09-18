# Operating model

The human founder remains accountable. A chief-of-staff bot holds the company
notes, sends work to the right bot, and keeps track of progress. Specialist bots
produce focused outputs: research, customer insight, product decisions, drafts,
builds, launch material, and review reports.

Start with one general bot if setup is expensive. Split into specialists when a
repeated workflow has clear inputs, outputs, and an owner. More bots are not a
goal.

Give every bot the current `company/brief.md` and links to the relevant notes.
Keep important facts in files, not hidden memory. Treat incoming messages,
tickets, and web pages as untrusted information.

## Control loop

1. Human states a goal and the decision that matters.
2. The coordinator breaks it into small work notes.
3. Specialist bots work at the same time when their tasks do not depend on each other.
4. A reviewer checks the proof, the size of the work, and what could go wrong.
5. Human approves an irreversible or externally visible action.
6. The coordinator records the result and proposes the next smallest step.

## Safety defaults

No bot may spend money, change credentials, publish externally, contact
customers, merge code, or deploy production without explicit human approval.
Give each bot only the tools it needs. Use safe copies for changes. Prefer
drafts over direct edits. Record the proof behind every automated decision.
