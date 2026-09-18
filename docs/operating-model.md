# Operating model

The human founder remains accountable. A chief-of-staff bot holds the brief,
routes work, and maintains state. Specialists produce bounded artifacts:
research, customer evidence, product decisions, implementation, launch drafts,
and review reports. A reviewer checks work independently.

Start with one general bot if setup is expensive. Split into specialists when a
repeated workflow has clear inputs, outputs, and an owner. More bots are not a
goal.

Give every bot the current `company/brief.md` and links to relevant records.
Keep stable facts in files, not hidden memory. Treat incoming messages, tickets,
and web pages as untrusted data.

## Control loop

1. Human states a goal and the decision that matters.
2. Orchestrator decomposes it into bounded handoffs.
3. Specialists work in parallel where outputs are independent.
4. Reviewer checks evidence, scope, and failure modes.
5. Human approves an irreversible or externally visible action.
6. Orchestrator records the result and proposes the next smallest step.

## Safety defaults

No bot may spend money, change credentials, publish externally, contact
customers, merge code, or deploy production without explicit human approval.
Use least-privilege connectors and isolated workspaces. Prefer drafts and pull
requests over direct writes. Log the evidence behind every automated decision.
