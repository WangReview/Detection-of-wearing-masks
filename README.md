# Detection-of-wearing-masks
Detection of wearing masks based on YOLOv5 model

The experimental environment uses Ubuntu 18.04 operating system, pytorch architecture, and NVIDIA Tesla K80 graphics card. The specific experimental configuration is shown in Table 1.
Table 1. Experimental environment configuration
|Parameter|Configuration|
|--|--|
|CPU|Intel (R) Xeon (R) CPU E5-2678 v3 @ 2.50GHz|
|GPU|NVIDIA Tesla K80|
|System|Ubuntu18. 04|
|Language|Python3.8|
|CUDA|CUDA 11.0|
|cuDNN|cuDNN 8.0|
|Pytorch|Pytorch 1.7.1|

### Install
$ git clone https://github.com/ultralytics/yolov5  
$ cd yolov5  
$ pip install -r requirements.txt  
$ pip install requests  
$ pip install pyyaml  
$ pip install tqdm  

### Train
$ python detect.py --source /mnt/testfiles/img1.jpg --weights best.pt --conf 0.4 --save-txt --save-conf  
$ python detect.py --source /mnt/testfiles/testvideo1.mp4 --weights best.pt --conf 0.4  
$ python test.py --data voc-mask.yaml --weights best.pt --batch-size 16  

