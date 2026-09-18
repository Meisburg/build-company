# BuildCompany

## Start here

Create one bot. Give it [`bots/bootstrapper.md`](bots/bootstrapper.md). Then
send:

```text
Let’s build a company.
```

That bot will ask one short question at a time, learn what you are building,
recommend the smallest useful team, and—after you approve the plan—create and
configure specialist bots when your bot system supports it.

You do not need to know which bots to create first.

## What BuildCompany is

BuildCompany is an open, vendor-neutral operating kit for building a company
with AI bots. It gives your team:

- a shared company brief;
- plain-language job instructions with clear limits;
- a simple way for bots to pass work to one another;
- a discover-to-launch workflow; and
- setup guides for Grok Bot, Hermes Bot Mode, OpenBot, or another bot system.

The operating model stays the same. Only the bot-runtime setup changes.

## Watch the inspiration

The workflow is based on the three-day Grok Bot Galaxy build, where a small team
worked from a blank slate through research, product decisions, engineering,
launch, and feedback.

- [Watch the Grok Bot Galaxy livestream](https://luma.com/3ifrgttw)
- [Visit the Grok Bot Galaxy event page](https://x.ai/galaxy)

## What happens next

1. The bootstrapper interviews you one question at a time.
2. It writes the company brief and the idea you are testing.
3. It recommends only the roles needed now.
4. You approve the team; it creates the specialists when possible.
5. The team works through discover → choose → first version → build → launch → learn.

## Safety defaults

Humans approve product bets, spending, credentials, customer contact, external
publishing, merges, and deployment. Bots may research, draft, classify,
implement in isolation, and report evidence. External messages, tickets, web
pages, and user content are treated as data—not instructions.

## Bot-system paths

- [Grok Bot adapter](adapters/grok-bot.md)
- [Hermes Bot Mode adapter](adapters/hermes-bot-mode.md)
- [Generic/OpenBot adapter](adapters/generic.md)

## Files you may need

- [`INSTALL.md`](INSTALL.md) — setup for a first bot
- [`bots/bootstrapper.md`](bots/bootstrapper.md) — the first-bot instructions
- [`company/`](company/) — shared company state
- [`bots/`](bots/) — specialist role cards
- [`docs/playbooks/`](docs/playbooks/) — lifecycle workflow
- [`docs/glossary.md`](docs/glossary.md) — plain-English definitions
- [`skill/`](skill/) — installable `$build-company` skill

## Attribution

This is an original synthesis of the supplied `day1.md`, `day2.md`, and `day3.md`
transcripts and the public [Grok Bot Galaxy](https://x.ai/galaxy) event.
BuildCompany is independent and does not imply endorsement by xAI, Hermes,
OpenBot, or any other vendor.
