#  YOLOv4：Optimal Speed and Accuracy of Object Detection #

https://hoya012.github.io/blog/yolov4/

https://medium.com/visionwizard

https://github.com/AlexeyAB/darknet

## abstract ##
논문 링크
* [You Only Look Once: Unified, Real-Time Object Detection](https://arxiv.org/abs/1506.02640)
* [YOLO9000: Better, Faster, Stronger](https://arxiv.org/abs/1612.08242)
* [YOLOv3: An Incremental Improvement](https://arxiv.org/abs/1804.02767)
* [YOLOv4: Optimal Speed and Accuracy of Object Detection](https://arxiv.org/abs/2004.10934)

해설 영상 링크
* [You Only Look Once: Unified, Real-Time Object Detection](https://www.youtube.com/watch?v=eTDcoeqj1_w)
* [YOLO9000: Better, Faster, Stronger](https://www.youtube.com/watch?v=6fdclSGgeio)
* [YOLOv3: An Incremental Improvement](https://www.youtube.com/watch?v=HMgcvgRrDcA)
* [YOLOv4: Optimal Speed and Accuracy of Object Detection](https://www.youtube.com/watch?v=CXRlpsFpVUE&feature=youtu.be)

필요조건
* Tensorflow 2.1.0
* tensorflow_addons 0.9.1 (required for mish activation)

## how to install ##
설치방법

[download](https://github.com/hunglc007/tensorflow-yolov4-tflite)

[yolov4 tutorial](https://youtu.be/sUxAVpzZ8hU)

<< best requirment >>
- (darkNet)[https://github.com/AlexeyAB/darknet] 
- CUDA 10.0
- cuDNN 7.4.3
- visual studio 2015
- opencv 4.1.0

[weight file](https://drive.google.com/file/d/1cewMfusmPjYWbrnuJRuKhPMwRe_b9PaT/view)

### yolov4 tutorial ###

1. Downloading DarkNet

- (Alexeyab darknet)[https://github.com/AlexeyAB/darknet]

2. Copying Open files into DarkNet

3. Copying CuDNN files into DarkNet

4. Changing the CuDNN version in DarkNet

5. Compile YOLOv4 with update CUDA version

6. compiling DarkNet

7. Run Detction on Images

8. Detection on Videos

https://blog.naver.com/shuna11/221979528693

### problem1 ###

include / library 디렉토리 잡는 법

프로젝트 > 속성 > VC++ directories
include directories
- ```(cuda 설치 디렉토리)\include```
- ```(opencv\빌드\인스톨)\include```

library directories
- ```(cuda 설치 디렉토리)\lib\x64```
- ```(opencv\빌드\인스톨)\x64\vc14\lib```

### problem2 ###

CUDA10.0.props & CUDA10.0.targets 잡는 법

line56

```<Import Project="(cuda 설치 디렉토리)\extras\visual_studio_integration\MSBuildExtensions\CUDA10.0.props"/>```

line308

```<Import Project="(cuda 설치 디렉토리)\extras\visual_studio_integration\MSBuildExtensions\CUDA10.0.targets"/>```
