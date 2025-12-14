# Image-Recogonization
The project helps to recognize the image confidence. how much the image is clarified.
!pip install -q ultralytics opencv-python-headless matplotlib pillow
from ultralytics import YOLO
import cv2
import matplotlib.pyplot as plt
from PIL import Image
from google.colab import files
uploaded =  files.upload()
file_name = list(uploaded.keys())[0]
print("Uploaded:", file_name)
model = YOLO('yolov8n.pt')
plt.figure(figsize=(12,8))
plt.imshow(cv2.cvtColor(annotated,cv2.COLOR_BGR2RGB))
plt.axis('off')
