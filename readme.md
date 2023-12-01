# 네잎클로버 탐지기 using Semantic Segmentation

## 데이터셋
[link](https://biomedicalcomputervision.uniandes.edu.co/publications/finding-four-leaf-clovers-a-benchmark-for-fine-grained-object-localization/)

## 라이브러리
* torch
* segmentation_models_pytorch
* albumentations
* monai

## 학습
1. oba.ipynb - 데이터증강
2. train.ipynb

## tflite 변환
torch_to_tflite.ipynb (코랩)

torch -> onnx -> tf -> tflite

## tflite tpu 변환
```
edgetpu_compiler -s filename.tflite
```