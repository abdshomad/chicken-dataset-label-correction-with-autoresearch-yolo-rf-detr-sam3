# Chicken Dataset Label Correction with Autoresearch, YOLO, RF-DETR and Meta SAM3

Meta-repo that pins a set of upstream projects used for **chicken detection / segmentation** and **dataset label correction** experiments (YOLO via Ultralytics, RF-DETR, and SAM3), plus a LabelMe-format dataset helper repo.

## What’s inside

- `chicken-detection-labelme-format/`: utilities + dataset in LabelMe format (upstream: `abdshomad/chicken-detection-labelme-format`)
- `ultralytics/`: YOLO training/inference toolkit (upstream: `ultralytics/ultralytics`)
- `rf-detr/`: Roboflow DETR implementation (upstream: `roboflow/rf-detr`)
- `sam3/`: Segment Anything Model v3 (upstream: `facebookresearch/sam3`)

## Clone (recommended)

Clone this repo **with submodules**:

```bash
git clone --recurse-submodules <THIS_REPO_URL>
cd chicken-dataset-label-correction-with-autoresearch-yolo-rf-detr-sam3
```

If you already cloned without submodules:

```bash
git submodule update --init --recursive
```

## Update submodules

Pull the latest commits from each upstream and record the new pins:

```bash
git submodule update --remote --recursive
```

## Notes

- Each submodule has its own install/run instructions—see the `README` in each directory.
- This repo does not currently include a single “runner” script; it primarily serves as a **reproducible checkout** of these upstream dependencies.

