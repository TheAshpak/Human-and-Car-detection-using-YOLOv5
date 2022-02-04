# Human-and-Car-detection-using-YOLOv5

YOLOv5 🚀 is a family of object detection architectures and models pretrained on the COCO dataset, and represents <a href="https://ultralytics.com">Ultralytics</a>
 open-source research into future vision AI methods, incorporating lessons learned and best practices evolved over thousands of hours of research and development.
</p>

</div>

## <div align="center">Documentation</div>

See the [YOLOv5 Docs](https://docs.ultralytics.com) for full documentation on training, testing and deployment.

## <div align="center">Quick Start Examples</div>

<details open>
<summary>Install</summary>

Clone repo and install [requirements.txt](https://github.com/ultralytics/yolov5/blob/master/requirements.txt) in a
[**Python>=3.7.0**](https://www.python.org/) environment, including
[**PyTorch>=1.7**](https://pytorch.org/get-started/locally/).

```bash
git clone https://github.com/ultralytics/yolov5  # clone
cd yolov5
pip install -r requirements.txt  # install
```

</details>

<details open>
<summary>Inference</summary>

Inference with YOLOv5 and [PyTorch Hub](https://github.com/ultralytics/yolov5/issues/36)
. [Models](https://github.com/ultralytics/yolov5/tree/master/models) download automatically from the latest
YOLOv5 [release](https://github.com/ultralytics/yolov5/releases).

```python
import torch

# Model
model = torch.hub.load('ultralytics/yolov5', 'yolov5s')  # or yolov5m, yolov5l, yolov5x, custom

# Images
img = 'https://ultralytics.com/images/zidane.jpg'  # or file, Path, PIL, OpenCV, numpy, list

# Inference
results = model(img)

# Results
results.print()  # or .show(), .save(), .crop(), .pandas(), etc.
```
</details>

## <div align="center">How To Use This Model</div>
 This Model is trained on data set containing Two categories **[Car,Person]**
<details open>
<summary>Steps to use this Model</summary>
 1) Clone repo, install dependencies and check PyTorch and GPU.
 use these commands to do it

 ```python
# !git clone https://github.com/ultralytics/yolov5  # clone
 
# %cd yolov5
 
# %pip install -qr requirements.txt  # install
 ```
2) Download weights from my drive
```python
# https://drive.google.com/file/d/1-5UOrK0zzpJEV5VAkp-h_v1USYbgdE-t/view?usp=sharing
```
3)Load this file in inference 
```bash
 !python detect.py --weights "best.pt" --img 640 --conf 0.25 --source "Image.jpg"
```
Done
 
</details>

## <div align="center">Recommondations</div>
<details open>
<summary>Recommondations</summary>
 
 ```
 - This weights are from only 160 epochs so you can start training your model with this weights as initial weights for better accuracy
 - Include mode data in training data with multiple daytime and low-light conditions for better accuracy 
 ```
 </details>
