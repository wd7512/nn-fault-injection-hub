# nn-fault-injection-hub  
A curated index of fault-injection tools and libraries for neural networks.  

## What’s this  
A central registry summarising open-source fault/injection frameworks, tools, and libraries targeting neural-network reliability analysis.  

## Why this repo exists  
- Fault-injection (FI) for neural networks is scattered across different frameworks, languages, and abstractions.  
- This repo makes it easier to discover, compare, and choose existing FI tools depending on your use case (framework, fault model, granularity, etc.).  
- It helps avoid duplication — and fosters standardisation of FI experiments in neural-network research.  

## How to use this repo  
1. Browse the table under **Existing tools & frameworks**.  
2. Filter by framework (e.g. PyTorch, TensorFlow), fault-granularity (e.g. bit-flip, neuron, weight), supported fault models.  
3. Click the GitHub links to view tool docs, licensing, and usage examples.  
4. Optionally contribute: add new tools, note compatibility, or contribute FI results / benchmarks.  

## Existing tools & frameworks  

| Name | Target Framework / Scope | Fault-injection Mode / Key Features | Notes / Status |
|---|---|---|---|
| **TensorFI** | TensorFlow (classic, graph-based) :contentReference[oaicite:1]{index=1} | Inject hardware/software faults (e.g. bit-flips) at operator level; supports DNNs (e.g. CNNs) :contentReference[oaicite:2]{index=2} | Tested on older TF versions; good for legacy / graph-based models |
| **TensorFI2** | TensorFlow 2 / Keras API :contentReference[oaicite:4]{index=4} | Static faults (layer-state) and dynamic faults (layer outputs); supports bit-flip, random or zero-replacement faults :contentReference[oaicite:5]{index=5} | More modern TF support; suitable if using TF2 + Keras |
| **PyTorchFI** | PyTorch :contentReference[oaicite:7]{index=7} | Runtime perturbation of weights or neurons during inference; supports DNN resilience analysis, object detection, classification, adversarial-robustness studies :contentReference[oaicite:8]{index=8} | Actively maintained; good general-purpose FI for PyTorch models |
| **PyTorchALFI** | PyTorch (application-level FI) :contentReference[oaicite:10]{index=10} | Adds automated instrumentation, data-loader wrapping, evaluation pipeline for FI campaigns (classification & object detection) :contentReference[oaicite:11]{index=11} | Archived / read-only as of Oct 2025 — may require fork for active use |
| **LLTFI** | ML applications + general C/C++ / LLVM-IR programs :contentReference[oaicite:13]{index=13} | Framework-agnostic fault-injection via lowering to LLVM IR — supports TensorFlow, PyTorch and native code :contentReference[oaicite:14]{index=14} | Useful for cross-framework or mixed-code settings; lower-level injection |
| **MRFI** | Deep Neural Networks (framework-agnostic / PyTorch-compatible) :contentReference[oaicite:16]{index=16} | Multi-resolution fault injection with configuration-based FI (no model rewriting), supports vulnerability analysis at different levels :contentReference[oaicite:17]{index=17} | Good for detailed, fine-grained fault-vulnerability studies |
| *[Optionally: future entries]* **SpikeFI** (for spiking neural networks) — see research pre-print :contentReference[oaicite:19]{index=19} | SNNs | Neuron/synapse fault models, supports transient & permanent faults, layer- and network-wide fault injection | Emerging; useful if working with neuromorphic / spiking networks |

## Proposed taxonomies / tags  
- **Framework**: PyTorch / TensorFlow / SNN / generic  
- **Granularity**: bit-flip / weight / neuron / operator / layer / IR-level  
- **Fault type**: hardware / software / transient / permanent / bit-flip / NaN / random / zero-replacement  
- **Usage scenario**: classification, object detection, inference-only, mixed code + ML  

## Contributing guidelines  
- If you know an FI tool not listed, send a PR adding it to the table (with link + brief description).  
- When adding a tool, please fill in the taxonomy tags (framework / granularity / fault type / scenario) for easier filtering.  
- If you upload FI experiment results, include environment, model architecture, fault-mode, seed, and metrics (e.g. silent data corruption rate, error-propagation, classification accuracy).  
- Use consistent formatting; keep table columns aligned; prefer lower-case, hyphen-separated file/folder names.  
- Maintain licensing compliance — include license info where available.  

## How to cite this repo  
If you use this repository (or benefit from its aggregated content) in publications, reports or experiments, please cite it as:  

