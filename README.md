# Blinky (with UART) Zephyr template for ESP32 DevKitC

## Environment

- Create workspace dir:

```
mkdir blinky_ws
cd blinky_ws
```

- Clone repository and change directory

- Use [Zephyr Nix](https://github.com/nix-community/zephyr-nix) shell:

```
nix develop
```

- Create Python Virtual environment with dependencies:

```
python -m venv .venv
source .venv/bin/activate
pip install -r requirements.txt
```

## Build

- Run `Build` task (or cmd-line equivalent)
- **Alternative** Neovim with `cmake-tools` plugin incremental build:
  - run `Configure` task
  - Ensure proper Zephyr CMake build folder is selected: `:CMakeSelectBuildDir build`
  - perform incremental CMake build: `:CMakeBuild`
- Ensure user is in `dialout` group for flash/console view operations

