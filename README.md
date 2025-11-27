# nn-fault-injection-hub
A curated index of fault-injection tools and libraries for neural networks.

| Name | PyTorch? | TensorFlow? | Example Added | Features |
|------|----------|-------------|---------------|----------|
| [PyTorchFI](https://github.com/pytorchfi/pytorchfi) | ✅ | ❌ | | Injects neuron/weight faults during inference; supports CNNs, detection models, robustness studies |
| [PyTorchALFI](https://github.com/IntelLabs/PyTorchALFI) | ✅ | ❌ | | Application-level FI with automated instrumentation; supports classification & detection (Archived but still useful) |
| [MRFI](https://github.com/fffasttime/MRFI) | ✅ | ❌ | | Multi-resolution FI; config-based fine-grained vulnerability analysis; framework-agnostic but PyTorch-friendly ([Paper](https://arxiv.org/abs/2306.11758)) |
| [TensorFI](https://github.com/DependableSystemsLab/TensorFI) | ❌ | ✅ | | Operator-level FI for graph-based TF models; bit-flips, random faults |
| [TensorFI2](https://github.com/DependableSystemsLab/TensorFI2) | ❌ | ✅ | | FI for TF2/Keras; static & dynamic layer faults, bit-flip/random/zeroed perturbations |
| [LLTFI](https://github.com/DependableSystemsLab/LLTFI) | ✅ | ✅ | | LLVM-IR-level FI for ML workloads; supports TF, PyTorch, and mixed C/C++ pipelines |


## Contribute
Submit a PR to add new FI tools or update entries.
