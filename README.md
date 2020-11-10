## YOLO_tensorflow

Tensorflow implementation of [YOLO](https://arxiv.org/pdf/1506.02640.pdf), including training and test phase.

### Directly use existing model data to detect
1. Download the YOLO model weight file and put it in`data/weight`
    [YOLO_small](https://drive.google.com/file/d/0B5aC8pI-akZUNVFZMmhmcVRpbTA/view?usp=sharing)
2. Put the RAP test data under'data'
3. Test
	```Shell
	$ python test_RAP.py
	```
#### Training with RAP training data
1. Modify configuration in `yolo/config.py`
2. Put the RAP dataset converted to VOC format under `data`
3. Training
	```Shell
	$ python train.py
	```
4. Test
	```Shell
	$ python test_RAP.py
	```

### Requirements
1. Tensorflow
2. OpenCV
