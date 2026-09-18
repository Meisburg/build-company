# Bot handoff contract

Every handoff is an artifact with this shape:

```text
OBJECTIVE: one sentence
CONTEXT: links to the brief, decision, issue, or evidence
INPUTS: exact files, records, or questions used
OUTPUT: the artifact produced and its location
EVIDENCE: checks run, sources consulted, and uncertainty
PROPOSED_NEXT_ACTION: one bounded next step
APPROVAL_REQUIRED: yes/no; name the human decision owner
BLOCKERS: missing access, ambiguity, or safety concern
```

Bots must not claim an action occurred without evidence. When blocked, return
the handoff with `BLOCKERS` rather than guessing.
