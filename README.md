# ICLR_MorphCurveVAE

A 2-stage pipeline to construct continuous morphological trajectories from collections of static, segmented 3D images -- specifically applied to a mitotic cell image dataset (Allen Institute WTC-11).

---

## Dataset

This project uses a subset of the **Mitotic Cell Annotations** dataset provided by the **Allen Institute for Cell Science (AICS)** and distributed via **Quilt Data**.

- **Original dataset homepage**:  
  https://open.quiltdata.com/b/allencell/packages/aics/mitotic_annotation

- **Original source organization**:  
  [Allen Institute for Cell Science](https://www.allencell.org/)

### Data Used in This Project

Only the following parts of the full dataset are required to reproduce the results of this project:

- `crop_seg/` — a folder of segmented 3D image crops
- `metadata.csv` — associated metadata for each image

These files are **restructured** into a format compatible with this pipeline, but **no changes were made to the image content or labels**.

---

## Data Access Instructions

To run the notebook on the dataset of interest:

1. Visit the original dataset page:  
   [https://open.quiltdata.com/b/allencell/packages/aics/mitotic_annotation](https://open.quiltdata.com/b/allencell/packages/aics/mitotic_annotation)

2. Download the `crop_seg/` folder and the `metadata.csv` file from the dataset package.

3. Place them into the following directory structure within this repository:

source_data/
├── crop_seg/
│ ├── image_001.tiff
│ ├── ...
├── metadata.csv

Once the files are placed in the `source_data/` directory as shown above, the notebook should run without modification.

---

## Citation and Attribution

If you use this code or data in your research, **please cite the original dataset authors**:

> Allen Institute for Cell Science. (2020). *Mitotic Cell Annotations (v0.1.1)* [Data set]. Quilt Data. https://open.quiltdata.com/b/allencell/packages/aics/mitotic_annotation

Additionally, cite this repository for the processing pipeline and analysis code.

---

## Environment Setup

This repository includes a `requirements.txt` file listing the Python packages needed.  
We recommend creating a fresh virtual environment.
