# Dentistry Crown Object Detection (YOLOv11)

This project trains a YOLOv11 dental crown detector using a Roboflow dataset.

## Dataset
The dataset is hosted on Roboflow and downloaded automatically inside the notebook:

```python
from roboflow import Roboflow
rf = Roboflow(api_key="YOUR_KEY")
project = rf.workspace("computer-vision-qnqjy").project("dentistry-crown-46s6n")
dataset = project.version(1).download("yolov11")
