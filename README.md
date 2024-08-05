# Multi-Constrained Discriminative Representations Network
⭐ This code has been completely released ⭐ 
<p align="center"> <img src="model.jpg" width="80%"> </p>

<summary>PREPARE</summary>

### 1. Dataset
- Download data for our experiment from [baiduyun]() (code: ). And the path of dataset is like that

```python
MIAYOLO
├── dataset
│   ├── CSRB
│   │   ├── train
│   │   │   ├── images
│   │   │   ├── labels
│   │   ├── val
│   │   │   ├── images
│   │   │   ├── labels
│   │   ├── test
│   │   │   ├── images
│   │   │   ├── labels
```
### 2. Install

```bash
pip install ultralytics
pip install -r requirements.txt
```
<summary>USAGE</summary>

## Train

```python
python train.py 
```
## Val
You can use our pretrained checkpoints for test process.
Download pre-trained model and put it in [here]() (code: ).

```python
yolo val model=MDRN.pt data=CSRB.yaml
```
## Predict
```python
yolo predict model=MDRN.pt source='xxx.jpg'
```

## Acknowledgements
This code is built on [YOLOv8 (PyTorch)](https://github.com/ultralytics/ultralytics). We thank the authors for sharing the codes.

