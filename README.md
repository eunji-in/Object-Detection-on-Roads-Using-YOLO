# Object Detection on Roads Using YOLO - 2023021274 차은지
## Copare with Denoised, Upscaled, Sharpened image

1. Project Results and Overview

Objective:
The goal of this project was to evaluate the impact of various image preprocessing techniques (upscaling, denoising, sharpening) on the performance of the YOLOv8 object detection model. By analyzing changes in detection accuracy, processing time, and memory usage, this project aimed to determine which preprocessing steps might enhance or hinder YOLOv8's performance.

Key Insights:
Original Image: Baseline results without any preprocessing.
Upscaling: Improved resolution sometimes enhanced detection for smaller objects but increased processing time significantly.
Denoising: Reduced noise in the image but occasionally resulted in lower detection accuracy.
Sharpening: Enhanced edges, which seemed to improve detection for certain object types.
This work provides valuable insights for optimizing YOLOv8 in real-world applications, particularly where preprocessing is feasible to boost model performance

2. Source Code

3. Performance Metrics

>test1

 Description|Processing Time (s)|Detected Objects
  ---|---|---
   Original| 0.355570|4|
   Upscaled| 0.363732|4|
   Denoised|0.372777|4|
  Sharpened|0.364677|1|

>test2

Description|Processing Time (s)|Detected Objects
  ---|---|---
   Original|0.910283|8|
   Upscaled|0.897763|8|
   Denoised|0.939744|8|
  Sharpened|0.817011|3|


>test3

  Description|Processing Time (s)|Detected Objects
  ---|---|---
   Original|0.571449|6|
   Upscaled|0.581833|6|
   Denoised|0.559759|5|
  Sharpened|0.573911|1|



  4. Installation and Usage

```python
pip install ultralytics
```
ultralytics : ultralytics에서 제공하는 라이브러리 이름으로 최신 YOLOv8 모델 지원한다. (객체 탐지, 분류, 세그멘테이션 기능)
