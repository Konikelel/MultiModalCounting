# CountGD source snapshot

This directory contains the Python source required to inspect and construct the
CountGD model used by this coursework. It was copied from the official CountGD
repository and remains under the included upstream `LICENSE`.

Included directories: `models/`, `groundingdino/`, `util/`,
`datasets_inference/`, plus `config/cfg_fsc147_vit_b.py`.

Large binary assets are intentionally not duplicated:

- `checkpoints/checkpoint_fsc147_best.pth` (about 1.2 GB)
- `checkpoints/bert-base-uncased/` (about 416 MB)

The source snapshot removes the instructor-specific path dependency, but the
large checkpoint and BERT assets remain required for the live-model tasks. The
notebook's cache mode is only a fallback for inspection.

Upstream: https://github.com/niki-amini-naieni/CountGD
