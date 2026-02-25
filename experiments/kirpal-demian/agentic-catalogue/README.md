# Agentic Catalogue

AI-powered product catalogue maintenance.

## How It Works

1. Agents crawl vendor product pages on schedule
2. Extract structured product data using LLM
3. Diff against current catalogue
4. Surface changes for review or auto-update

## Architecture

- Crawler: Playwright + Claude for extraction
- Orchestration: LangGraph
- Storage: PostgreSQL with vector search
