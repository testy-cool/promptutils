# promptutils

Utilities for working with Large-Language-Model (LLM) prompts.

## Installation

Install directly from GitHub using your preferred installer. With **uv** (recommended)::

```bash
uv pip install git+https://github.com/yourusername/promptutils.git@main
```

Using plain **pip** works as well::

```bash
pip install git+https://github.com/yourusername/promptutils.git@main
```

Replace `yourusername` and branch/ref as necessary (e.g., `@v0.1.0`).

## Usage

```python
from promptutils import clean_prompt

raw = """
    # This is a comment line
        Some indented prompt line.

        Another line.
"""

print(clean_prompt(raw))
# -> "Some indented prompt line.\n\nAnother line."
```

## Development

1. Create and activate a virtual environment (Windows example):

```bash
uv init
a
workon .venv
uv pip install -e .[dev]
```

2. Run tests (if added later)::

```bash
pytest -q
```
