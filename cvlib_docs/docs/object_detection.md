## detect_common_objects
```
detect_common_objects(image, confidence=0.5, nms_thresh=0.3, model='yolov3', enable_gpu=False)
```

**Arguments**

- **image:** input image (numpy array, BGR order, `dtype` - `uint8`)
- **confidence:** confidence threshold to filter the detections below the threshold value (ranges from 0 to 1. default value 0.5)
- **nms_thresh:** confidence threshold to filter the detections (ranges from 0 to 1. default value 0.5)
- **model:** object detection model to use for inference. possible options `yolov3` or `yolov3-tiny` pretrained on [coco](cocodataset.org) dataset. (default model - `yolov3`)
- **enable_gpu:** flag to use available GPU (if you have compiled OpenCV with CUDA from source)

**Returns**

- **bbox:** list of list containing bounding box co-ordinates for detected objects.
- **labels:** list of labels for detected objects.
- **confidences:** list of confidence scores for detected objects.