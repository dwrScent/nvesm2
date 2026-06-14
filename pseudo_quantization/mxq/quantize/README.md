# Quantization utilities

This directory contains experimental quantization functions and analysis scripts
used by the NVESM2 evaluation flow.

- `exp.py`: standalone experiments for comparing MX/NV/NVESM2-style quantizers,
  including MSE, entropy, kurtosis, and histogram analysis.
- `awq/run_awq.py`: AWQ calibration helpers for collecting layer inputs and
  deriving scale/clip settings on supported Hugging Face models.
- `awq/inpu_anal.py`: activation/input distribution analysis utilities,
  including 3D surface plots, histograms, entropy metrics, and NVESM2 checks.

Most scripts assume local model checkpoints, CUDA, and temporary tensors under
`dump/`; adjust those paths before running them on a new machine.
