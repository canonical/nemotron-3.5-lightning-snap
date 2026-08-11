<!--
# This is the name of the snap. The name that is registered on the snap store and also the name of the cli command.
snap-name: nemotron-3-5-lightning
# This name is just a friendly name for the snap, it can be used in the documentation
snap-friendly-name: Nemotron 3.5 Lightning
# URL to model card from the model publisher
model-card: https://huggingface.co/nvidia
# The port that the inference snap will use for its API server.
http-port: 8346
# The port that the inference snap will use for its webui server.
webui-http-port: 8348
# Optimizations
engines: cpu, nvidia-gpu
-->

# Nemotron 3.5 Lightning inference snap
[![nemotron-3-5-lightning](https://snapcraft.io/nemotron-3-5-lightning/badge.svg)](https://snapcraft.io/nemotron-3-5-lightning)

NVIDIA Nemotron 3.5 Lightning is a customizable open model built for fast, always-on agents that run anywhere, from edge devices to local systems, datacenters, and the cloud.

Use this snap to quickly install an optimized environment for local inference with Nemotron 3.5 Lightning.

The snap includes the following hardware-optimized inference engines:

* cpu: Optimized for x64 and ARM (armv8, armv9) CPUs
* nvidia-gpu: CUDA-enabled GPU acceleration

The most suitable engine is automatically selected based on the available hardware.

#### Install
```
sudo snap install nemotron-3-5-lightning
```

#### Run
```
nemotron-3-5-lightning
```

> [!TIP]
> Some accelerators require extra [drivers](https://documentation.ubuntu.com/inference-snaps/how-to/setup/drivers/) to be usable with this snap.

## Resources

📚 **[Documentation](https://documentation.ubuntu.com/inference-snaps/)**, learn how to use inference snaps

💬 **[Discussions](https://github.com/canonical/inference-snaps/discussions)**, ask questions and share ideas

🐛 **[Issues](https://github.com/canonical/inference-snaps/issues)**, report bugs and request features

## Build and install from source

Clone the repo:
```shell
git clone https://github.com/canonical/nemotron-3.5-lightning-snap
cd nemotron-3.5-lightning-snap
```

Initialize the development environment:
```shell
make init
```

Build and install snap:
```shell
make build
make install
```
