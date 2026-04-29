# tmux for prompt_agent: Repair and Replay Evaluation

## Purpose

This document records the research framing behind the static GitHub Pages site. The project studies how tmux can be adapted for prompt_agent as a durable terminal substrate for agentic work.

## Research Question

Which traces show that prompt_agent repaired terminal work through evidence rather than repeated prompting alone?

## Working Thesis

Evaluation should connect prompt updates to concrete terminal evidence, making repair behavior inspectable at pane, command, and artifact levels.

## Design Claims

- Fault injection introduces missing files, failing commands, and stale panes.
- Replay analysis links prompt changes to observed shell state.
- Scoring rewards verifiable repair paths over final-state luck.

## Evaluation Lens

- Evidence-backed repair rate
- Replay interpretability
- Prompt drift during long sessions


## Threats to Validity

- Terminal state can be over-instrumented, causing an adapter to measure artifacts of the harness rather than real agent behavior.
- A final successful artifact may hide poor recovery behavior, repeated command attempts, or fragile focus management.
- Agent-specific adapters can become difficult to compare unless trace schemas remain explicit and documented.

## Hero Image Source

The GitHub Pages hero image uses the shared tmux CUA screenshot, copied into `docs/assets/hero.png` at its original 1484x1060 PNG resolution.
