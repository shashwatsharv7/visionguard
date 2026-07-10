# VisionGuard

VisionGuard is a step-by-step computer vision project for industrial image anomaly detection.

The goal is to understand the full workflow, starting with simple image exploration and classical image-processing baselines before moving toward deep learning methods.

## Current Phase

Phase 0: repository setup and dataset planning.

In this phase we only want a clean project skeleton:

- keep source data out of git
- use notebooks for early exploration
- document the dataset plan
- avoid deep learning until the image data is understood

## Dataset Plan

The first dataset will be [MVTec AD](https://www.mvtec.com/research-teaching/datasets/mvtec-ad), a standard industrial anomaly detection benchmark.

Why this dataset:

- it contains product and texture categories
- training images are defect-free
- test images include normal and defective examples
- pixel-level defect masks are available for evaluation
- it is widely used in anomaly detection research

For the first exploration steps, start with one visually simple category instead of the full dataset. Good first candidates are `bottle`, `capsule`, or `hazelnut`.

Expected local layout after downloading one category:

```text
data/
  raw/
    mvtec_ad/
      bottle/
        train/
        test/
        ground_truth/
```

Do not commit dataset files to git.

## Project Roadmap

1. Repo setup
2. Dataset exploration
3. Image loading and visualization
4. Normal vs defective image understanding
5. Mask understanding
6. Simple image-processing baseline
7. Thresholding and connected components
8. Classical anomaly score
9. Evaluation metrics
10. Deep learning baseline
11. Patch-based anomaly detection
12. Heatmaps
13. Robustness under lighting changes
14. API/demo
15. Docker
16. README and portfolio polish

## Notes

This project should stay readable and practical. Early code should prefer clarity over clever abstractions.
