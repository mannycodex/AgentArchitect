# Agent Architect

A meta-agent for designing, specifying, and shipping other agents.

Agent Architect turns a vague idea ("I want an agent that does X") into a complete, buildable agent specification, then guides you through testing and deployment. It does not build the downstream agent inside its own context. It produces a spec you can paste into a Claude Project, a Claude Code subagent, or an API worker and run immediately.

## What's in this repo

- [`agent-architect.md`](./agent-architect.md) — the full Agent Architect system prompt, operating principles, four-phase workflow, patterns library, and house style.

## Workflow at a glance

1. **Discovery** — up to three questions to pin down job, trigger, and definition of done.
2. **Challenge** — pressure-test scope, cheapest viable version, and the most likely failure mode.
3. **Specification** — fill out the structured agent card (purpose, runtime, system prompt, inputs, outputs, tools, guardrails, eval cases, deployment notes, open questions).
4. **Test and iterate** — dry-run the eval cases, revise, then ship.

## Patterns library

Research, Triage, Drafting, Review, Extraction, Orchestrator. See `agent-architect.md` for the full descriptions and failure modes.

## How to use it

1. Open `agent-architect.md`.
2. Paste the contents into a Claude Project, a Claude Code subagent file, or an API system prompt.
3. Start the conversation with the agent idea you want to build.

## Citation

If you use or adapt Agent Architect, please cite it:

```
Cordero, M. (2026). Agent Architect: A meta-agent for designing, specifying,
and shipping other agents. GitHub. https://github.com/mannycodex/AgentArchitect
```

BibTeX:

```bibtex
@misc{cordero2026agentarchitect,
  author       = {Cordero, Manuel},
  title        = {Agent Architect: A meta-agent for designing, specifying, and shipping other agents},
  year         = {2026},
  howpublished = {\url{https://github.com/mannycodex/AgentArchitect}}
}
```

## License

This work is licensed under a [Creative Commons Attribution-NonCommercial 4.0 International License (CC BY-NC 4.0)](./LICENSE). You are free to share and adapt the material for non-commercial purposes, as long as you give appropriate credit using the citation above. Commercial use requires separate permission from the author.
