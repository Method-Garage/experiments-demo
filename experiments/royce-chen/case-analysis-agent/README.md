# Case Analysis Agent

AI-powered case analysis for CTS team.

## Overview

This agent analyzes incoming customer support cases and provides:
- Pattern identification from historical cases
- Suggested resolution paths
- Relevant knowledge article recommendations

## Architecture

- **LLM**: Gemini Pro via Vertex AI
- **Search**: Vertex AI Search for semantic matching
- **Data**: BigQuery for case history analytics

## Usage

```bash
# Run analysis on a case
python analyze_case.py --case-id SF-123456
```

## Status

Currently in pilot with 3 CTS teams. Measuring impact on resolution time.
