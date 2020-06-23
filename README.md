## MobileNetv2-YOLOv3-SPP Darknet 

A darknet implementation of MobileNetv2-YOLOv3-SPP detection network

Network|VOC mAP(0.5)|Resolution|Inference Time(GTX2080ti)|FLOPS|Weight size
:---:|:---:|:---:|:---:|:---:|:---:
MobileNetV2-YOLOv3-SPP|71.7|416|5ms|5.5BFlops|14.2

*emmmm...这个懒得训练，mAP就凑合这样吧
## ***Darknet Group convolution is not well supported on some GPUs such as NVIDIA PASCAL!!! The MobileNetV2-YOLOv3-SPP	inference time is 100ms at GTX1080ti, but RTX2080 inference time is 5ms!!!***
## Mobile inference frameworks benchmark (4*ARM_CPU)
Network|VOC mAP(0.5)|COCO mAP(0.5)|Resolution|Inference time (NCNN/Kirin 990)|Inference time (MNN arm82/Kirin 990)|FLOPS|Weight size
:---:|:---:|:---:|:---:|:---:|:---:|:---:|:---:
MobileNetV2-YOLOv3-Lite|72.61|35.2|320|33 ms|18 ms|2.1BFlops|9.8MB
MobileNetV2-YOLO-Tiny|61.17|30.4|304|26 ms|11 ms|1.5BFlops|3.9MB
MobileNetV2-YOLO-Nano|&|&|304|& ms|& ms|0.5BFlops|1.3MB
[YOLO-Tiny](https://pjreddie.com/darknet/yolov2/)|57.1|&|416|& ms|& ms|6.97BFlops|60.0MB
[YOLOv3-Tiny-Prn](https://github.com/AlexeyAB/darknet#pre-trained-models)|&|33.1|416|44 ms|& ms|3.5BFlops|18.8MB
[YOLO-Nano](https://github.com/liux0614/yolo_nano)|69.1|&|416|& ms|& ms|4.57BFlops|4.0MB

* Darknet Train Configuration: CUDA-version: 10010 (10020), cuDNN: 7.6.4,OpenCV version: 4 GPU:RTX2080ti
* Support mobile inference frameworks such as NCNN&MNN

## MobileNetV2-YOLOv3-Lite-COCO Test results
![image](https://github.com/dog-qiuqiu/MobileNetv2-YOLOV3/blob/master/data/predictions.jpg)


## NCNN conversion tutorial
* benchmark:https://github.com/Tencent/ncnn/tree/master/benchmark
* darknet2ncnn: https://github.com/Tencent/ncnn/tree/master/tools/darknet
## NCNN Android Sample
* 白嫖中....
## MNN conversion tutorial
* 待完成
## Reference&Framework instructions
https://github.com/AlexeyAB/darknet
