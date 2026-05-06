## Getting Started

> Based on the official [K230 Linux SDK build instructions](https://github.com/kendryte/k230_linux_sdk/tree/4885c98d0b888bd123969f2c3b4fc771db3c06a4#build).

---

### 1. Clone

```bash
git clone --recursive git@github.com:Iari-Lab/camera_software.git
cd camera_software
```

> [!NOTE]
> The `--recursive` flag is required to initialize all submodules.

---

### 2. Build the Docker image

```bash
docker compose build k230-build
```

> [!TIP]
> Only needed once, or when the `Dockerfile` or its dependencies change.

---

### 3. Start the build environment

```bash
docker compose run k230-build
```

---

### 4. Build the SDK

Inside the container:

```bash
make CONF=k230d_canmv_defconfig
```
