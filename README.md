# Face Mask Detector

![example](https://github.com/ddikodroid/yolov3-face-mask-detector/blob/master/detection/detections.jpg)

The file require to make face mask detector based on YoloV3.
Download all files and put it in darknet directory.

## Usage
### Training
1. Open powershell
2. Go to darknet directory
3. Type this code in powershell
```
./darknet.exe detector train data/obj.data cfg/yolov3-custom.cfg darknet53.conv.74
```

After finished the training, the weight files will be saved in /backup folder

### Detection
1. Open powershell
2. Go to darknet directory
3. Type this code in powershell
```
#Image File
./darknet.exe detector test data/obj.data cfg/yolov3-custom.cfg backup/yolov3-custom_last.weights [file-path/filename].jpg

#Video
./darknet.exe detector test data/obj.data cfg/yolov3-custom.cfg backup/yolov3-custom_last.weights [file-path/filename].mp4 -out_filename [output filename you want].avi
```

## Detection in Video

![example](https://github.com/ddikodroid/yolov3-face-mask-detector/blob/master/detection/detections.gif)
