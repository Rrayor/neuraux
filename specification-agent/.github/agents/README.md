# Specification Agent Pack

This folder contains a fresh custom-agent mesh for specification authoring.

Agents:
- `specification-orchestrator.agent.md` (entrypoint)
- `specification-context-gatherer.agent.md`
- `specification-question-scout.agent.md`
- `specification-question-validator.agent.md`
- `specification-decision-steward.agent.md`
- `specification-decision-validator.agent.md`
- `specification-lane-validator.agent.md`
- `specification-writer.agent.md`
- `specification-glossary-steward.agent.md`
- `specification-memory-steward.agent.md`
- `specification-memory-validator.agent.md`
- `specification-progress-manager.agent.md`
- `specification-traceability-manager.agent.md`
- `specification-quality-validator.agent.md`
- `specification-consistency-checker.agent.md`

Conventions:
- Agent names start with `Specification - ...`
- Specialist agents are `user-invokable: false`
- Orchestrator is the only workflow controller
- Specialist-to-specialist calls are not allowed
- Progress tracker bootstrap is orchestrator-triggered and executed by progress manager
- Decision state memory (`docs/specification/.decisions.md`) is orchestrator-triggered and maintained by decision steward

Packaging note:
- This agent pack is self-contained and does not require `SPECIFICATION.md` at runtime.
