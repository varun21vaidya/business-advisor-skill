# Business Advisor

[![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](LICENSE)

An agent skill for deciding what to do next in a business. Use it to evaluate a new offer, improve cash flow, diagnose a sales problem, or plan a change in operations. It adapts to your industry, country, business stage, and resources.

## Quick start

Install the skill using the [Skills CLI](https://github.com/vercel-labs/skills). Run this from your project and select your agent when prompted.

```sh
npx skills add varun21vaidya/business-advisor-skill --skill business-advisor
```

You can also use [GitHub CLI](https://cli.github.com/manual/gh_skill_install). This example targets Claude Code. Replace `claude-code` with your agent's ID, such as `codex`, `cursor`, `github-copilot`, `gemini-cli`, or `opencode`.

```sh
gh skill install varun21vaidya/business-advisor-skill business-advisor --agent claude-code
```

For manual installation, copy the complete [business-advisor](skills/business-advisor/) folder into your harness's skills directory and keep the folder name. The skill follows the [Agent Skills specification](https://agentskills.io/specification) and uses Markdown and relative references. It runs without scripts, API keys, or MCP servers. The `agents/openai.yaml` file provides optional Codex display metadata.

Start a fresh session if your agent needs to reload skills, then ask it to use the **business-advisor** skill. Use the harness's native invocation if available, for example `$business-advisor` in Codex or `/business-advisor` in Claude Code. If your harness has no skill loader, point it to the skill instructions and tell it where to find the adjacent references, or provide those files directly.

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

> Use business-advisor to compare fixed-price projects with monthly retainers for our consulting business. Show the effects on capacity, margins, and cash timing.

> Use business-advisor to find why qualified leads aren’t converting. Use our pipeline data to propose one test and decide what would count as improvement.

> Use business-advisor to build a 13-week cash forecast for a retailer with delayed supplier shipments and seasonal sales. Ask for the figures you need.

## How it works

The skill uses the context you provide and asks focused questions when missing information could change the recommendation. It distinguishes observed evidence from assumptions, compares practical options, and proposes a next step with a way to measure the result.

- [Skill instructions](skills/business-advisor/SKILL.md) define when to ask questions and how to turn advice into action.
- [Operating playbook](skills/business-advisor/references/operating-playbook.md) covers methods and worked examples.
- [Source guide](skills/business-advisor/references/source-guide.md) lists research starting points and explains how to check local applicability.

## Contributing

Open an issue or pull request with an example prompt, the gap you found, and the behavior you’d expect. For new methods or regulatory guidance, include a primary source and note where it applies.

## License

[MIT](LICENSE)
