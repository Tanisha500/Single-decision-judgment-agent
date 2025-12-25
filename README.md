# Single-decision-judgment-agent

This repository contains a judgment-governed internal decision agent designed to evaluate whether to act or deliberately remain silent in situations involving ambiguous intent, incomplete authority, and potential irreversible harm.

The system prioritizes restraint, authority boundaries, and long-term risk prevention over responsiveness or optimization.

# What This Agent Does

1. Interprets a scenario without assuming intent
2. Identifies tempting but unauthorized actions
3. Evaluates irreversible risks of action vs silence
4. Chooses a final posture (act or remain silent)
5. Produces two submission-ready artifacts:
- decision_note.txt

- decision_state.json

Silence is treated as a deliberate, terminal decision, not a delay.

# Workflow Overview

Execution Flow:

1. Manual trigger initiates evaluation
2. Scenario and authority constraints are injected
3. Judgment reasoning is performed by an LLM
4. Outputs are parsed into structured artifacts
5. Artifacts are exported as text and JSON files

The workflow is intentionally minimal to avoid optimization bias.

# Output Files
1. decision_note.txt

Explains:

- the tempting action
- why it appears reasonable
- why the agent acts or remains silent
- what irreversible harm is prevented

2. decision_state.json

# How the Agent Reasons (Short Note)

1. The agent does not optimize for politeness or reassurance
2. It refuses to assume authority it does not have
3. It treats implied commitments as irreversible risk
4. It allows uncertainty to remain unresolved
5. Silence is selected only when it protects the system

# What the Agent Deliberately Avoids

- Asking clarifying questions
- Making implied commitments
- Escalating without irreversible risk
- Providing customer-facing reassurance
- Optimizing outcomes under uncertainty

# Design Philosophy

A decision is not safe because it acts — it is safe because it knows when not to.

# Screenshot
<img width="1334" height="451" alt="image" src="https://github.com/user-attachments/assets/65a87b6f-3828-4aee-afa8-0362f9eb28f5" />
