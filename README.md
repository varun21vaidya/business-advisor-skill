# Business Advisor

[![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](LICENSE)

An agent skill for deciding what to do next in a business. Use it to evaluate a new offer, improve cash flow, diagnose a sales problem, or plan a change in operations. It adapts to your industry, country, business stage, and resources.

## Quick start

Install for your Codex account with Git:

```sh
git clone https://github.com/varun21vaidya/business-advisor-skill.git ~/.codex/skills/business-advisor
```

Start a fresh Codex session and invoke `$business-advisor`. If you use a custom Codex home, put the clone in its `skills/business-advisor` directory. For another tool that supports Agent Skills, copy the skill folder into that tool’s skills directory and keep `SKILL.md` and `references/` together.

## When to use it

| Decision | What to ask for |
| --- | --- |
| Strategy and business models | Compare customer segments, pricing models, or routes to market. |
| Finance and budgeting | Build a cash forecast or estimate contribution margin and break-even volume. |
| Sales and marketing | Diagnose a pipeline or funnel, draft outreach, or plan a channel test. |
| Customer research and analytics | Design interviews or experiments and define what evidence would change the decision. |
| Projects and operations | Find a bottleneck, plan a rollout, or compare manual work with buying or building software. |
| Leadership and negotiation | Prepare for a negotiation, delegate an outcome, or structure a feedback conversation. |

## Example prompts

> $business-advisor Compare fixed-price projects with monthly retainers for our consulting business. Show the effects on capacity, margins, and cash timing.

> $business-advisor Help me find why qualified leads aren’t converting. Use our pipeline data to propose one test and decide what would count as improvement.

> $business-advisor Build a 13-week cash forecast for a retailer with delayed supplier shipments and seasonal sales. Ask for the figures you need.

## How it works

The skill uses the context you provide and asks focused questions when missing information could change the recommendation. It distinguishes observed evidence from assumptions, compares practical options, and proposes a next step with a way to measure the result.

- [Skill instructions](SKILL.md) define when to ask questions and how to turn advice into action.
- [Operating playbook](references/operating-playbook.md) covers methods and worked examples.
- [Source guide](references/source-guide.md) lists research starting points and explains how to check local applicability.

## Contributing

Open an issue or pull request with an example prompt, the gap you found, and the behavior you’d expect. For new methods or regulatory guidance, include a primary source and note where it applies.

## License

[MIT](LICENSE)
