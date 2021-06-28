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




#安装requests
pip install requests
安装yaml
pip install pyyaml
安装tqdm
pip install tqdm

成功命令，在/mnt/yolov5-master下执行
1、测试图片
python detect.py --source /mnt/testfiles/img1.jpg --weights best.pt --conf 0.4 --save-txt --save-conf
2、测试视频
python detect.py --source /mnt/testfiles/testvideo1.mp4 --weights best.pt --conf 0.4
3、性能统计
python test.py --data voc-mask.yaml --weights best.pt --batch-size 16
