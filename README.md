# LLM Zoomcamp 2026 Code

This repository serves as a clean starting point for the LLM Zoomcamp 2026 project. It is designed to help you build, experiment with, and extend Python-based LLM applications in a structured and professional way.

## Overview

The project includes a minimal Python setup powered by `uv`, making it easy to manage dependencies and run your code consistently. It is ideal for learning, prototyping, and building small AI-powered applications.

## Project Structure

- `main.py` — the main entry point for the project
- `pyproject.toml` — project metadata and dependency configuration
- `README.md` — project documentation

## Getting Started

### Prerequisites

- Python 3.13 or newer
- `uv` installed on your system

### Installation

1. Clone the repository:
   ```bash
   git clone <repository-url>
   cd llm-zoomcamp-2026-code
   ```

2. Create and activate the environment with `uv`:
   ```bash
   uv venv
   source .venv/bin/activate
   ```

3. Install dependencies:
   ```bash
   uv sync
   ```

### Running the Project

Run the main script with:

```bash
uv run python main.py
```

## Notebook Setup (Jupyter)

If you are using `notebook.ipynb` in VS Code and encounter a `ModuleNotFoundError` for packages like `google-generativeai`:

1.  **Select the correct kernel:** Click on the kernel picker in the top right corner of the notebook.
2.  **Choose the environment:** Select **"Python (llm-zoomcamp)"**. This kernel is linked to the project's virtual environment where all dependencies are installed.

If you don't see that kernel, you can re-register it by running:
```powershell
.\.venv\Scripts\python.exe -m ipykernel install --user --name llm-zoomcamp-2026-code --display-name "Python (llm-zoomcamp)"
```

## Development Notes

You can add new packages with:

```bash
uv add requests minsearch openai jupyter python-dotenv google-generativeai
```

This project is intentionally lightweight, so it can be expanded easily as your work grows.

## License

This project is intended for educational and experimental use.