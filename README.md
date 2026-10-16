# build-company

> Early preview: a portable set of instructions and templates for starting a
> company with AI bots.

## Why this exists

Grok Bot hosted a three-day **Galaxy livestream** showing how a small team could
start with a blank slate and build a company in public. They worked through the
real sequence: finding an idea, learning what customers need, deciding what to
make, building a first version, launching it, and learning from feedback.

I saved the three-day transcripts and turned the useful parts into this project.
The goal is simple: give someone a way to start their own company with one bot,
then let that bot help design and create the rest of the team.

BuildCompany began with Grok Bot, but the underlying workflow is not specific to
Grok. It can also be adapted for Hermes Bot Mode, OpenBot, or any future system
that lets people create and coordinate AI bots.

Watch the original [Grok Bot Galaxy livestream](https://luma.com/3ifrgttw) or
visit the [Galaxy event page](https://x.ai/galaxy) to see the inspiration.

## Start here

Create one bot. Give it [`bots/bootstrapper.md`](bots/bootstrapper.md). Then
send:

```text
Let’s build a company.
```

That bot will ask one short question at a time, learn what you are building,
recommend the smallest useful team, and—after you approve the plan—create and
configure specialist bots when your bot system provides that capability. If it
cannot create bots, it gives you ready-to-copy instructions.

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

## See the experience

```text
Founder: Let’s build a company.

Bootstrapper: What do you want to build, and who is it for?

Founder: A service that helps local restaurants get better photos.

Bootstrapper: Step 1 of 5 complete. I understand the customer and problem.
Next: what proof do you already have that restaurants want this?
```

The bot keeps asking focused questions, shows progress, proposes the team, and
waits for your approval before setting anything up.

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

“OpenBot” here means OpenBot or any other bot system that supports named bots,
shared instructions, and communication between bots. The generic adapter is
the correct starting point when your system is different.

## What works today

- The bootstrapper prompt and plain-language specialist role cards are ready to
  copy into a bot system.
- The shared company files and discover-to-launch workflow are ready to use.
- Grok Bot and Hermes Bot Mode have translation guides; exact account setup and
  bot-creation behavior depends on the current product version.
- Other systems can use the generic adapter without changing the workflow.

This project does not currently provide a hosted service, API integration, or
one-click bot creation across every platform.

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
