# nn-fault-injection-hub
A curated index of fault-injection tools and libraries for neural networks.

## PyTorch Frameworks
### **PyTorchFI**
- **Repo:** github.com/pytorchfi/pytorchfi  
- **Features:** Injects neuron/weight faults during inference; supports CNNs, detection models, robustness studies.

### **PyTorchALFI**
- **Repo:** github.com/IntelLabs/PyTorchALFI  
- **Features:** Application-level FI with automated instrumentation; supports classification & detection.  
- **Note:** Archived but still useful.

### **MRFI**
- **Paper:** arxiv.org/abs/2306.11758  
- **Features:** Multi-resolution FI; config-based fine-grained vulnerability analysis; framework-agnostic but PyTorch-friendly.

## TensorFlow Frameworks
### **TensorFI**
- **Repo:** github.com/DependableSystemsLab/TensorFI  
- **Features:** Operator-level FI for graph-based TF models; bit-flips, random faults.

### **TensorFI2**
- **Repo:** github.com/DependableSystemsLab/TensorFI2  
- **Features:** FI for TF2/Keras; static & dynamic layer faults, bit-flip/random/zeroed perturbations.

## Framework-Agnostic / Lower-Level
### **LLTFI**
- **Repo:** github.com/DependableSystemsLab/LLTFI  
- **Features:** LLVM-IR-level FI for ML workloads; supports TF, PyTorch, and mixed C/C++ pipelines.

## Contribute
Submit a PR to add new FI tools or update entries.
