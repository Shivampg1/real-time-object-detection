# real-time-object-detection
Object Detection Model: YOLOv3
You Only Look Once or more popularly known as YOLO is one of the fastest real-time object
detection algorithm (45 frames per second) as compared to the R-CNN family (R-CNN, Fast R-CNN,
Faster R-CNN, etc.)
The R-CNN family of algorithms uses regions to localise the objects in images which means the
model is applied to multiple regions and high scoring regions of the image are considered as object
detected.
Instead of selecting some regions, YOLO approaches the object detection problem in a completely
different way.
It forwards the entire image to predict bounding boxes and their probabilities only once through the
neural network.
The authors have also improved the network by making it bigger and taking it towards residual
networks by adding shortcut connections.

Object Detection Model: YOLOv3
First, it divides the image into a 13×13 grid of cells. The size of these 169 cells varies depending on the input size. For a
416×416 input size, the cell size was 32×32. Each cell is responsible for predicting the number of boxes in image.
For each bounding box, the network also predicts the confidence that the bounding box actually encloses an object, and the
probability of the enclosed object being a particular class.
Most of these bounding boxes are eliminated because their confidence is low or because they are enclosing the same object
as another bounding box with a very high confidence score. This technique is called non-maximum suppression.
