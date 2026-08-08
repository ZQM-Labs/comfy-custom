# comfy-custom

Fork of ComfyUI (v0.27.0) with custom nodes, API extensions, execution modifications, and deployment tooling.

## About

`comfy-custom` is a customized ComfyUI deployment that preserves upstream compatibility while layering in custom nodes, middleware, API endpoints, model management, subgraph replacement, and a frontend asset pipeline. It is intended as an operational image-generation stack rather than a plugin drop-in.

## Installation

```bash
python -m venv .venv
.\.venv\Scripts\pip install -r requirements.txt
python main.py
```

Web UI: `http://127.0.0.1:8188`

## Usage

- Launch `main.py` to start the ComfyUI server.
- Place workflows in `input/`, outputs in `output/`.
- Custom nodes and blueprints are loaded from `custom_nodes/` and `blueprints/`.
- API server extensions live under `api_server/`.

## Features

- Upstream ComfyUI 0.27.0 execution core
- Custom node library under `custom_nodes/`
- API server and middleware extensions
- Model manager, subgraph replace manager, and node replace manager
- Alembic-backed schema migrations
- Deployment manifests and service wrappers
- Hook breaker, latent preview, and quantization utilities
- CUDA malloc diagnostics helper

## License

MIT — see [LICENSE](LICENSE).

## Contact

zqmcomputing@gmail.com
