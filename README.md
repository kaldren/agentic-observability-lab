# Agent Observability Lab

Experimental repo for building and testing an end-to-end observability and continuous improvement workflow for AI agents and skills.

## Goal

Build this lifecycle:

```text
Agent / Skill
    ↓
OpenTelemetry tracing
    ↓
Azure Application Insights
    ↓
Microsoft Foundry Observability
    ↓
Agent and Skill Evaluations
    ↓
Production failures become regression tests
    ↓
Agent / Skill changes through GitHub PRs
    ↓
GitHub Actions run evaluations
    ↓
Compare candidate vs baseline
    ↓
Human approval
    ↓
Deploy
```

## Experiments

* Trace agent runs, model calls, tool calls, handoffs, latency, tokens and errors.
* Track agent, skill, prompt and Git commit versions in every trace.
* Create evaluation datasets for agents and skills.
* Test task completion, instruction adherence, tool selection and tool accuracy.
* Test skill triggering, non-triggering, coexistence and instruction following.
* Convert failed production traces into regression cases.
* Run evaluations automatically in GitHub Actions.
* Block PRs when agent or skill quality regresses.
* Experiment with an agent that analyzes failures and proposes Skill changes through PRs.
* Add continuous production evaluation and quality monitoring.

## Stack

* Microsoft Azure
* Microsoft Foundry
* Azure Application Insights
* Azure Monitor
* OpenTelemetry
* GitHub
* GitHub Actions
* Custom Agents
* Agent Skills
