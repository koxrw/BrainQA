# BrainQA:Transformer-Driven Invariant Grounding for 3D Brain imaging Question Answering

## Usage
### 1、Data
Including ADNI, OASIS and AIBL

### 2、Preprocessing
All MRI images undergo standardized preprocessing to ensure anatomical consistency across subjects and datasets. First, non-brain tissues are removed using the Brain Extraction Tool, followed by spatial normalization to the MNI152 template with 1 mm isotropic resolution. Intensity non-uniformities are corrected via N4 bias-field correction, and the resulting images are visually inspected for quality control. Subsequently, each preprocessed MRI volume is segmented into 32 anatomical regions of interest using the atlas, which provides the anatomical basis for generating the atlas-level ROI tokens Batlas.

### 3、Run
run 'model_train.py'. (The code for the model module will be open-sourced during the manuscript accepted.)

### 4、Model
model:
![model](./images/model.pdf "model")


result:
![result](./images/result.png "result")

energy:
![energy](./images/Energy.png "energy")

TSNE:
![TSNE](./images/TSNE.png "TSNE")


