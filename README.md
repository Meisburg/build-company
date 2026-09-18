# BuildCompany

Build a company with a team of AI bots—without having to guess which bots to
create, what to tell them, or how to make them work together.

BuildCompany is an open, vendor-neutral operating kit for turning an idea into
validated product, first launch, and a learning loop. It is designed to work
with Grok Bot, Hermes Bot Mode, OpenBot, and future agent platforms.

## The experience

You start with one bot. Upload the BuildCompany skill or give it the
`bots/bootstrapper.md` instructions, then say:

> Let’s build a company.

That bot walks you through a short founder interview. It learns what you want to
build, recommends only the roles you need right now, creates the shared company
workspace, and gives you setup instructions for each specialist bot. If your
runtime can create bots, it can help create them; otherwise it gives you
copyable setup packets.

You do not need to understand the whole system or choose seven bots up front.

## Watch the inspiration

The system is inspired by the three-day Grok Bot Galaxy build, where a small
team worked from a blank slate through research, product decisions, engineering,
launch, and feedback.

- [Watch the Grok Bot Galaxy livestream](https://luma.com/3ifrgttw)
- [Visit the Grok Bot Galaxy event page](https://x.ai/galaxy)

The livestream is useful even if you never use Grok Bot: it demonstrates the
underlying operating pattern of a human-led team of specialized agents.

## What the bootstrapper creates

- A concise company brief and current hypothesis
- A recommended human decision owner and chief-of-staff bot
- Only the specialist roles the current stage requires
- Shared files for decisions, evidence, backlog, metrics, and feedback
- Handoff instructions so bots can pass work reliably
- A validate-to-launch workflow: discover → bet → MVP → build → launch → learn
- Runtime-specific setup guidance for Grok Bot, Hermes, OpenBot, or another system

## Why use it?

Most multi-agent setups fail because every bot has a different picture of the
company. BuildCompany fixes that with shared context, explicit handoffs, small
work items, evidence trails, and human approval at the points that matter.

The resulting team can research markets, understand customers, define an MVP,
build reviewable changes, draft launch experiments, triage feedback, and propose
improvements without silently changing company policy.

## Safety by default

Bots may research, draft, classify, implement in an isolated workspace, and
report evidence. Humans remain responsible for product bets, spending,
credentials, customer contact, external publishing, merges, and deployment.
Untrusted messages, tickets, web pages, and user-generated content are treated
as data—not instructions.

## Works with your runtime

BuildCompany is a portable set of instructions and artifacts, not a competing
bot platform:

- **Grok Bot:** use bots, connectors, repositories, and routines.
- **Hermes Bot Mode:** map roles to persistent profiles, bot chats, groups, and
  routines.
- **OpenBot or another system:** map the same role contracts to named agents,
  shared files, messaging, schedules, tools, and review gates.

The operating model stays the same; only the runtime translation changes.

## Repository map

| Path | What it gives you |
| --- | --- |
| `bots/bootstrapper.md` | The first-bot setup instructions |
| `company/` | Brief, decisions, evidence, backlog, metrics, feedback |
| `bots/` | Specialist role cards with permissions and stop conditions |
| `docs/playbooks/` | Validate-to-launch workflow |
| `docs/` | Handoff, safety, and adapter contracts |
| `adapters/` | Generic, Hermes, and Grok translations |
| `skill/` | Installable `$build-company` skill |

## Get started

Clone the repository or upload the skill to your preferred bot runtime. Start
the first bot with the bootstrapper and say: **“Let’s build a company.”**

## Attribution

The workflow is an original synthesis of the supplied `day1.md`, `day2.md`, and
`day3.md` transcripts and the public [Grok Bot Galaxy](https://x.ai/galaxy)
event. BuildCompany is independent and does not imply endorsement by xAI,
Hermes, OpenBot, or any other vendor.
