# LensNet: CNN vs ViT for Dark Matter Substructure Classification

Classifying strong gravitational lensing images into 3 classes (no substructure / CDM subhalo / vortex-axion type) and comparing CNN and Vision Transformer models on the same data, same split, same metrics.

> Status: 🚧 just started. This README gets updated as each phase finishes.

## Goal
One honest comparison table: which architecture works better on lensing images, at what cost (params, training time)?

## Results (fill as you go)

| Model | Params | Macro ROC-AUC | Accuracy | Train time |
|---|---|---|---|---|
| Baseline CNN | - | - | - | - |
| ResNet-style CNN | - | - | - | - |
| ViT (from scratch) | - | - | - | - |
| ViT (pretrained, fine-tuned) | - | - | - | - |

## Roadmap
- [ ] Phase 1: data exploration + `Dataset`/`DataLoader` + train/val split
- [ ] Phase 2: baseline CNN (self-built), metrics + confusion matrix
- [ ] Phase 3: ResNet-style CNN, ablation (depth / augmentation)
- [ ] Phase 4: ViT from scratch, then pretrained fine-tune
- [ ] Phase 5: comparison table, loss curves, final write-up

## Repo layout
```
data/        dataset (not committed, see .gitignore)
notebooks/   exploration and experiments
src/         dataset, models, train loop, metrics
results/     plots, tables, saved metrics
LOG.md       dated progress log with numbers
```

## Setup
```bash
python -m venv .venv
source .venv/bin/activate
pip install -r requirements.txt
```

## Dataset
Source: ML4Sci DeepLense test dataset (add exact link and class counts here after Phase 1).

## Tech
Python, PyTorch, scikit-learn, NumPy, Matplotlib
