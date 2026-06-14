# NVESM2

This repository contains the NVESM2 quantization and hardware evaluation flow.
It combines post-training quantization experiments, accelerator simulation, and
RTL area/power analysis for comparing NVESM2 with related low-precision
accelerator baselines.

## Structure

- `pseudo_quantization/`: PTQ and model evaluation scripts.
- `simulator/`: BitFusion-style mixed-precision accelerator simulator with
  CACTI-backed SRAM modeling.
- `rtl_area_power/`: RTL, synthesis scripts, and area/power reports for PE and
  quantization-engine units.

Forked from M2XFP:
https://github.com/SJTU-ReArch-Group/M2XFP_ASPLOS26
