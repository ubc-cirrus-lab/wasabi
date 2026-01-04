# wasabi (Integrated Wasm Serving Stack)

This repository integrates two components into a single experimental stack for resource-efficient serverless WebAssembly serving:

- **WasmBox:** a WebAssembly runtime providing lightweight execution and isolation.
- **Resource-Aware Serving:** a modified version of Knative Serving with added resource-aware mechanisms and metrics collection.

Both components are included as git submodules and can be developed and evaluated independently or together.

## Repositories

- **WasmBox**  
  [https://github.com/ubc-cirrus-lab/WasmBox](https://github.com/ubc-cirrus-lab/WasmBox)
  
  WebAssembly runtime with CPU and memory isolation support.

- **Resource-Aware Serving (Knative-based)**  
  [https://github.com/ubc-cirrus-lab/resource-aware-knative-serving](https://github.com/ubc-cirrus-lab/resource-aware-knative-serving)
  
  A fork of Knative Serving extended with resource-aware scheduling, serving logic, and metrics collection.

## Getting Started

Clone this repository **with submodules**:

```bash
git clone --recurse-submodules <repo-url>
```

If already cloned:

```bash
git submodule update --init --recursive
```

**Note:** This repository serves as an integration and entry point, and further setup, build, and deployment documentations are provided in each submodule.
