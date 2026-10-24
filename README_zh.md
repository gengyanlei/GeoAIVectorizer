# GeoAIVectorizer
### GeoAIVectorizer, Intelligent vectorization of geological grid maps; 地质图件AI矢量化

<p align="center">
    <a href="./README.md">English</a> |
    <a href="./README_zh.md">简体中文</a>
</p>

## 1-地质图件AI矢量化软件(GeoAIVectorizer) 简介
* 地质图件智能(自动)矢量化：采用深度学习、GIS、图像处理、软件、地质学、等学科技术知识进行研发
* 2026.11.01 正式发布 v2.0 功能支持：地理配准投影、更加强大的OCR能力(分块预测、灰度图预测、roi区域过滤)、更好的线矢量化能力、地球化学成果反演到原始(更多复杂的功能)、简化线、网格线过滤...
<!-- ![GeoAIVectorizer-v2.0](./data/geoaivectorizer1.png) -->
* <p align="center"> <img src="./data/geoaivectorizer1.png" width="600" alt="GeoAIVectorizer-v2.0"> </p>
* 2024.12.10 正式发布 v1.0功能支持：地质图点状符号检测识别矢量化、文本点矢量化、线矢量化(AI-OCR辅助去干扰项)、面矢量化、地质专业OCR数据集+模型、简化线
* <p align="center"> <img src="./data/geoaivectorizer2.png" width="600" alt="GeoAIVectorizer-v2.0"> </p>

## 2-应用
* v1.0
* 中国地质调查局某些单位
* 中国各省地质单位
* 目前已推广应用中国5省 10+ 家地质单位
* v2.0
* 进行中

## GeoAIVectorizer v1.0与v2.0 差异对比
| 对比项 | v1.0 | v2.0 |
| --- | --- | --- |
| 在线or离线 | 离线 | 离线 |
| 开发方式 | 人工代码设计编写 | cursor + trae 代码结构重构+生成; 代码接管99%, 数据集+模型独立 |
| Python | 3.9 | 3.12 |
| PaddleOCR | 2.6 (ppocrv4) | 3.7 (ppocrv6) |
| GDAL | 3.4 | 3.12 |
| GeoPandas | 0.14 | 1.2 |
| GUI 框架 | QT for Python (PySide6) | QT for Python (PySide6) |
| OpenCV | opencv-python 4.5 | opencv-python 5 |
| 点状符号检测 | 自研CV算法 | 无 |
| CUDA | 11.2 | 12.9 |
| 地理配准投影 | 不支持 | 支持 |
| OCR 能力 | 基础识别(地质专业数据集+模型) | 分块预测、灰度图预测、ROI 区域过滤 |
| 线矢量化 | AI-OCR 辅助去干扰项 | 更强的线矢量化能力 |
| 网格线过滤、简化线等其它功能 | 部分支持 | 支持 |
| 地球化学成果反演 | 不支持 | 支持(更多复杂功能) |


### v3.0 (TODO 2027)
* 计划中(更加复杂的功能)
* qwen3-vl or not
* mcp or not
* agent or not
* Qgis or rustGIS
* ollama or xinference
* fastapi or not
* docker or not