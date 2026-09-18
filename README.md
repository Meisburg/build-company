# BuildCompany

A vendor-neutral starter kit for building a company with a small team of AI bots.
It turns the useful operating pattern shown in the Grok Bot Galaxy three-day
build into portable role cards, shared artifacts, lifecycle playbooks, and
runtime adapter guidance.

This is a playbook and set of prompts, not an orchestration service. It works
with any bot network that provides named agents, shared context, messaging, and
optionally scheduled routines and repository access.

## Quick start

1. Copy `company/` into your project or business workspace.
2. Complete `company/brief.md` with a human.
3. Start with `chief-of-staff`, `researcher`, `product`, `builder`, and
   `reviewer`; add other roles only when their inputs and outputs are distinct.
4. Give every bot the same brief and require `docs/handoff-contract.md`.
5. Run `docs/playbooks/validate-to-launch.md`.
6. Choose a runtime translation in `adapters/`.

Humans approve product bets, spending, external communication, merges, and
production changes. The companion Codex skill in `skill/` turns a short intake
into a customized copy of these artifacts.

## Layout

| Path | Purpose |
| --- | --- |
| `company/` | Shared company state and operating records |
| `bots/` | Role cards with permissions, outputs, and stop conditions |
| `docs/playbooks/` | Validate-to-launch workflow gates |
| `docs/` | Handoff, adapter, and safety contracts |
| `adapters/` | Generic, Hermes, and Grok runtime translations |
| `skill/` | Installable Codex/agentskills-compatible skill |

## Attribution

This is an original synthesis of the supplied `day1.md`, `day2.md`, and
`day3.md` transcripts and the public [Grok Bot Galaxy](https://x.ai/galaxy)
event page. It is independent and does not imply vendor endorsement.
