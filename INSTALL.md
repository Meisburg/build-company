# Install BuildCompany

Start with one bot. Do not set up the whole team manually.

## 1. Add the bootstrapper

Give your first bot the contents of [`bots/bootstrapper.md`](bots/bootstrapper.md)
or install the `skill/` package if your runtime supports skills.

## 2. Start the conversation

Send:

```text
Let’s build a company.
```

The bot will ask one short question at a time, recommend the smallest useful
team, and wait for approval before creating specialist bots.

## 3. Choose your runtime path

- **Grok Bot:** read [`adapters/grok-bot.md`](adapters/grok-bot.md).
- **Hermes Bot Mode:** read [`adapters/hermes-bot-mode.md`](adapters/hermes-bot-mode.md).
- **OpenBot or another runtime:** read [`adapters/generic.md`](adapters/generic.md).

If your runtime can create bots, the bootstrapper can create and configure the
approved specialists. If it cannot, it produces copyable setup packets.

## 4. Keep the next action visible

The bot should always tell you what step is complete and give you one next
action. If it gives you a long unranked plan, ask: “What is the next action I
can finish in two minutes?”
