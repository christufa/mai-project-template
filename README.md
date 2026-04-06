# mai-project-template

A GPU-enabled data science dev container backed by a nightly-published image on `ghcr.io`.

---

### 1. Set mounts


In .devcontainer/devcontainer.json, specify a mount to store data or cache if necessary.

---

## Configuration reference



| Variable | Default | Description |
|---|---|---|
| `GHCR_REPO` | *(required)* | GitHub org/repo, e.g. `myorg/myrepo` |
| `IMAGE_TAG` | `main` | Image tag to pull. Use a semver tag (e.g. `v1.2.3`) to pin |
| `CONDA_ENV_NAME` | `ds` | Conda environment name |
| `CONTAINER_NAME` | `ds-dev` | Docker container name |
| `NVIDIA_VISIBLE_DEVICES` | `all` | GPUs exposed to the container |
| `CUDA_VISIBLE_DEVICES` | `all` | GPUs visible to CUDA. Set to `0` to pin to first GPU |
| `MEMORY_LIMIT` | `80g` | Container memory cap |
| `NETWORK_MODE` | `bridge` | Docker network mode. Use `host` if needed |
| `HOST_DATA_PATH` | `./data` | Host path mounted to `/workspace/data` |
| `HOST_CACHE_PATH` | `./cache` | Host path mounted to `/workspace/.cache` |

---
