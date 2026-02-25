# AI Experiment Rules

This document defines the guardrails for AI experiments at Autodesk.

## Required for All Experiments

1. **No hardcoded credentials** - Use environment variables or secret managers
2. **No PII in prompts** - Anonymize or aggregate data before sending to LLMs
3. **Logging enabled** - All LLM calls must be logged for audit

## Platform-Specific Rules

### ChatGPT Custom GPTs
- Must use approved Actions only
- Cannot access internal APIs directly
- Upload only anonymized/sample data

### Cursor / Claude Code
- Follow standard code review process
- Include `.cursorrules` or `CLAUDE.md` with project context
- Tests required for production use

### Copilot Studio
- Approved connectors only
- No direct database access
- Must go through MuleSoft for integrations

## Status Progression

- **idea**: Concept only, no code written
- **prototype**: Working demo, internal testing
- **pilot**: Limited production use, 1-3 teams
- **scaling**: Approved for broader rollout
- **scaled**: Fully deployed, standard process

## Getting Help

Questions? Reach out in #ai-builders or contact the AI Coordination team.
