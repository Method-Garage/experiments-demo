# Autodesk AI Experiments

This repository is the source of truth for AI experiments across the organization.

## Structure

```
experiments/
├── .platform/           # Rules and schemas
│   ├── rules.md         # AI experiment guardrails
│   └── experiment-schema.yaml
├── experiments/         # All experiments by builder
│   └── {builder-name}/
│       └── {experiment}/
│           ├── experiment.yaml  # Metadata
│           └── README.md        # Documentation
├── patterns/            # Reusable patterns (coming soon)
└── backlog/             # Workflow automation requests
```

## Adding an Experiment

1. Create folder: `experiments/{your-name}/{experiment-name}/`
2. Add `experiment.yaml` with required fields
3. Add `README.md` with documentation
4. Push to main branch

The crawler will automatically index your experiment within 1 hour.

## Workflow Requests

Have a workflow you'd like automated? Add a YAML file to `backlog/` describing:
- The problem
- Current state
- Desired state
- Success metrics

## Questions?

Contact the AI Coordination team or post in #ai-builders.
