# Benchmarking Type Inference for Large JavaScript Monorepos

**Accepted at COLM 2026 — Accepted (oral).** Camera-ready code release.

## Overview

This repository contains the reference implementation of *Benchmarking Type Inference for Large JavaScript Monorepos*.
It includes the data pipeline, the training entry point, the evaluation
harness and the experiment configurations used for the camera-ready results.

## Repository layout

```
src/          model, data pipeline, training and evaluation code
experiments/  base and ablation configurations
notebooks/    result analysis
results/      reported metrics
tests/        unit tests
```

## Setup

```bash
python -m venv .venv && source .venv/bin/activate
pip install -r requirements.txt
```

## Reproducing the main result

```bash
python -m src.train --config experiments/base.yaml
python -m src.evaluate --config experiments/base.yaml
```

## Citation

```bibtex
@inproceedings{okafor2026benchmarking,
  title     = {Benchmarking Type Inference for Large JavaScript Monorepos},
  booktitle = {Proceedings of COLM 2026},
  year      = {2026}
}
```
