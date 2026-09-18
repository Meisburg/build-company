# Hermes Bot Mode adapter

This is a translation guide, not a required dependency. Hermes Bot Mode presents
named profiles as persistent bots with bot chats and routines.

| Portable role | Hermes profile | Typical surface |
| --- | --- | --- |
| Chief of staff | `chief-of-staff` | canonical bot chat |
| Researcher | `researcher` | direct chat and read-only routine |
| Customer voice | `customer-voice` | feedback room or direct chat |
| Product | `product` | decision and backlog drafts |
| Builder | `builder` | repository/worktree handoffs |
| Growth | `growth` | launch drafts and metric summaries |
| Reviewer | `reviewer` | independent review chat |

Use routines for recurring briefs, evidence scans, and improvement proposals;
keep them read-only by default. Put the shared `company/` folder in the
workspace each profile can access, and pass links rather than stale prompt
copies. Use peer or group messaging only for the handoff contract. Confirm
current Hermes permissions and connection behavior in its official docs before
enabling a connector.

Reference: [Hermes Bot Mode documentation](https://github.com/NousResearch/hermes-agent/tree/main/website/docs/user-guide).
