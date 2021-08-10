# Predictive Mask Annotation using pretrain models (video)

Suppose we are developing a new labeling tool to annotate masks in a video.Labeling all the frames of a video with a great accuracy takes a lot of time and cost. In order to make annotation process faster, we need to use semi-automated or automated labelling methods. Therefore, we need to implement a method to annotate an object in a few frames and the tool keep detecting that object in next frames. Ultimately, we want the tool to annotate all video frames itself after annotating a few frames.

### previous work flow on this research topic

- [The surprising impact of mask-head architecture on novel class segmentation](https://arxiv.org/pdf/2104.00613.pdf)

- [You Only Look Once: Unified, Real-Time Object Detection](https://arxiv.org/pdf/1506.02640.pdf)

- [OverFeat: Integrated Recognition, Localization and Detection using Convolutional Networks](https://arxiv.org/pdf/1312.6229.pdf)

- [Mask R-CNN](https://arxiv.org/pdf/1703.06870.pdf)



### open source repositories on this grand

- [TensorFlow Object Detection API](https://github.com/tensorflow/models/tree/master/research/object_detection)


### mask_rcnn_inception_resnet_v2_atrous_coco_2018_01_28

- In the second method, a combination of two models is used. faster RCNN - InceptionResNet V2
  + Deep MAC. In this two-part model, the box around the objects is first obtained by faster RCNN
  - InceptionResNet V2, and after this step, the object mask is applied by Deep MAC. This
  method is highly dependent on the first step, which is to find the boxes, and if the boxes are
  determined with high accuracy, deep mac can do its job well. 
  
- main video

https://user-images.githubusercontent.com/78655282/125610848-b75e9593-9cb7-4408-aad1-27344bea044c.mp4

- output video

https://user-images.githubusercontent.com/78655282/125618593-79d03991-3488-4d61-81e7-2ef23aacb7db.mp4


### Faster RCNN + InceptionResNet V2 + Deep MAC

In the second method, a combination of two models is used. faster RCNN - InceptionResNet V2 + Deep MAC. In this two-part model, the box around the objects is first obtained by faster RCNN - InceptionResNet V2, and after this step, the object mask is applied by Deep MAC. This method is highly dependent on the first step, which is to find the boxes, and if the boxes are determined with high accuracy, deep mac can do its job well. To improve the result, you can use other models such as YOLOv3-spp and YOLOv3-608, which are much better at finding boxes and finally their work speed is high.In this method, processing every 4 seconds for each frame,
and for 74 frames of time equivalent to 296 seconds

- main video

https://user-images.githubusercontent.com/78655282/125610848-b75e9593-9cb7-4408-aad1-27344bea044c.mp4

- output video

https://user-images.githubusercontent.com/78655282/125618476-a597ed29-b7bd-446c-9440-8600bbd9372d.mp4







