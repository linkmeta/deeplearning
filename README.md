# deeplearning
# 一、数据获取与使用
## 1.数据获取
### 公开数据集：
```
    MNIST
    CIFAR10/CIFAR100
    The PASCAL
    ImageNet
    Microsoft COCO
```
### 自建数据集
```
  摄像头采集
  数据众包
  数据爬虫
  图片爬虫
     Image Downloader
     Annie
```
## 2. 数据整理
### 统一格式
```
    python 使用opencv处理
```
### 错误数据去除
```
    模型筛选
    人工筛选
```
### 相似图处理,hash去重算法
### 数据预处理
### 数据标注
```
    开源工具Lableme
```
## 3. 数据增强
```
    从有限的数据产生无数种变化
    提高模型泛化能力
    
```
### 单样本数据增强
```
    几何变换 - 翻转、旋转、裁剪、缩放
    颜色操作 - 噪声、模糊、颜色扰动
```
### 多样本数据增强
```
    Synthetic Minority Over-sampling technique
    Sample Pairing
    Mixup
```
### 无监督数据增强
```
    生成模型，生成器与判别器对抗学习，生成器学习真实数据的概率分布
    增强规则学习，Autoaugmentation,学习已有数据增强操作的组合，不同的任务，需要不同的数据增强操作
```
# 二、表情图像分类任务
## 1.图像分类基础
### 什么是图像分类
```
    跨物种分类
    细粒度分类
    实例级分类
```
### 图像分类模型
```
    MNIST与LeNet5
    深度学习里程碑，ImageNet与AlexNet
```

### 分类模型架构演变
```
    VGG->GoogleNet->ResNet->MobileNet
```    
 
## 2.数据与模型准备
### 任务：基于嘴唇的表情识别
```
    公开数据集：KDEF,RaFD,EmotioNet
    人脸数据集：Celeba
    
 ```
### 数据预处理
```
    OpenCV 人脸检测
    Dlib关键点检测
    嘴唇区域裁剪
```
### 模型选择
```
    Google 分组卷积模型MobileNet
        28层，Depthwise和Pointwise组成，3x3卷积
        结构简单，性能稳定
        预训练模型多
```
## 3.模型训练与测试
### 
