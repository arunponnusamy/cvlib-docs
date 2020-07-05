## detect_gender
```
detect_gender(face, enable_gpu=False)
```

**Arguments**

- **face:** cropped face region (numpy array, BGR order, `dtype` - `uint8`)
- **enable_gpu:** flag to use available GPU (if you have compiled OpenCV with CUDA from source)

**Returns**

- **labels:** list of labels. `['male', 'female']`
- **confidences:** list of confidence score for each label (float, between 0 to 1).