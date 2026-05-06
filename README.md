## Getting Started

### 1. Clone (recursive)

```bash
git clone --recursive git@github.com:Iari-Lab/camera_software.git
cd camera_software
```

> The `--recursive` flag is required to initialize all submodules.

### 2. Build the container

```bash
docker compose build k230-build
```

> This step only needs to be run once, or whenever `Dockerfile` or dependencies change.
