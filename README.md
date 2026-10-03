# AI Engineering

My workspace for AI engineering: LLM applications, retrieval-augmented generation (RAG),
agents and evaluation. Each project lives in its own folder under [`projects/`](projects).

> [!NOTE]
> Just getting started. The first projects are on their way.

## Structure

```text
projects/      one folder per project, each with its own README
pyproject.toml shared tooling: Python version, Ruff and pytest settings
```

## Setup

Requires [uv](https://docs.astral.sh/uv/).

```bash
uv sync                          # create .venv with the dev tools
uv run pre-commit install        # lint and format on every commit
cp .env.example .env             # add API keys locally; .env is git-ignored
```

## Conventions

- Each project gets its own folder with a README explaining the problem, approach and results.
- Secrets stay in `.env` and never get committed. GitHub secret scanning and push protection are on.
- Code is linted and formatted with Ruff, tested with pytest and checked in CI on every push and pull request.

## Planned

- [ ] LangChain vs LangGraph: the same agent workflow built both ways and compared

## License

[MIT](LICENSE)
