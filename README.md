# Predictive Mask Annotation using mask_rcnn_inception_resnet_v2 on video

Suppose we are developing a new labeling tool to annotate masks in a video. Labeling all the frames of a video with great accuracy takes a lot of time and cost. In order to make the annotation process faster, we need to use semi-automated or automated labeling methods.

### mask_rcnn_inception_resnet_v2_atrous_coco_2018_01_28

In this repository, I have tried to make a pipeline using the mask_rcnn_inception_resnet_v2 pretrained model to detect and mask vehicles on the highway. Also, you can use this pipeline for detecting objects that are in [coco_2018_01_28 labels](https://tech.amikelive.com/node-718/what-object-categories-labels-are-in-coco-dataset/) labels. 

### Results

- main video

https://user-images.githubusercontent.com/78655282/125610848-b75e9593-9cb7-4408-aad1-27344bea044c.mp4

- output video

https://user-images.githubusercontent.com/78655282/125618593-79d03991-3488-4d61-81e7-2ef23aacb7db.mp4


### References 

- [Mask R-CNN](https://arxiv.org/pdf/1703.06870.pdf)

### Open source repositories on this grand

- [TensorFlow Object Detection API](https://github.com/tensorflow/models/tree/master/research/object_detection)
