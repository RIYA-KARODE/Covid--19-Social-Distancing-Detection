# Covid--19-Social-Distancing-Detection
This social distancing detection tool was developed to detect the safety distance between people in public spaces. 

The deep CNN method and computer vision techniques are employed in this work. Initially, an open-source object detection network based on the YOLOv4 algorithm was used to detect the pedestrian in the video frame. From the detection result, only pedestrian class was used and other object classes are ignored in this application. Hence, the bounding box best fits for each detected pedestrian can be drawn in the image, and these data of detected pedestrians will be used for the distance measurement. 

For camera setup, the camera is captured at fixed angle as the video frame, and the video frame was treated as perspective view are transformed into a two-dimensional top-down view for more accurate estimation of distance measurement. 

In this methodology, it is assumed that the pedestrians in the video frame are walking on the same flat plane. Four filmed plane points are selected from frame and then transformed into the top-down view. 

The location for each pedestrian can be estimated based on the top-down view. The distance between pedestrians can be measured and scaled. Depending on the preset minimum distance, any distance less than the acceptable distance between any two individuals will be indicated with red lines that serve as precautionary warnings. The work was implemented using the Python programming language.

