# YOLO11-AND-SAM2
YouTube Tutorial: https://youtu.be/YkmeBa807a8

This project uses deep learning to automatically detect and segment brain tumors in medical images. It combines a custom-trained YOLO (You Only Look Once) model for object detection with Meta's Segment Anything Model (SAM) for fine-grained segmentation.
The YOLO model is trained on MRI images labeled with tumor types like glioma and meningioma. It first detects tumors by drawing bounding boxes around them. These detected regions are then passed to SAM, which produces precise pixel-level masks outlining the exact shape of each tumor.
By merging fast detection (YOLO) with accurate segmentation (SAM), the system provides detailed visual outputs useful for diagnosis and research. The final images include both bounding boxes and segmentation masks, highlighting tumor locations and boundaries.

Environment setup:
Ultralytics recommend to install pytorch first from official website as per your cuda version- 
https://pytorch.org/get-started/locally.

pip install torch torchvision torchaudio --index-url https://download.pytorch.org/whl/cu121

pip install Ultralytics

![meningioma_3](https://github.com/user-attachments/assets/204b1e14-642f-4da3-8cb3-7da34dc9601b)
