# People-detection-tracking-and-counting
Object detection and tracking is implemented using YOLOv4, DeepSort and Tensorflow. YOLOv4 is a state of the art algorithm that uses deep convolutional neural networks to perform object detections. The output of YOLOv4 is fed into Deep SORT (Simple Online and Realtime Tracking with a Deep Association Metric) in order to create a highly accurate object tracker. Counters are implemented to count the total number of unique people throughout the video and using a reference line, the number of people passing from left to right is counted.

During execution, the video shows the tracking of each person(bounding box) with their respective ID’s. The Unique Person count in the entire video and the count of people moving from left to right is displayed in the terminal after the execution.

Libraries Used : OpenCV, TensorFlow, Numpy, Pillow


     To Execute the code - Run the following commands in Terminal/Command Prompt :
1) python save_model.py --weights ./data/yolov4-tiny.weights --output ./checkpoints/yolov4- tiny-416 --input_size 416 --model yolov4 --tiny
2) python track_objects.py --weights ./checkpoints/yolov4-tiny-416 --score 0.3 --video ./data/ test.mp4 --model yolov4




***Screenshots*** :


![image](https://user-images.githubusercontent.com/41203054/120713910-2ce73380-c4e0-11eb-9c81-b81295372b59.png)
![image](https://user-images.githubusercontent.com/41203054/120713928-32447e00-c4e0-11eb-8bfa-54f64b938703.png)
