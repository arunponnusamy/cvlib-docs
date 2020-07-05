## detect_face
```
detect_face(image, threshold=0.5, enable_gpu=False)
```

**Arguments**

- **image:** input image (numpy array, BGR order, `dtype` - `uint8`)
- **threshold:** confidence threshold to filter the detections (ranges from 0 to 1. default value 0.5)
- **enable_gpu:** flag to use available GPU (if you have compiled OpenCV with CUDA from source)

**Returns**

- **faces:** list of list containing bounding box co-ordinates for each detected face.
- **confidences:** list of confidence scores for each detected face.