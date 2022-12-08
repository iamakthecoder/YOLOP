# YOLOP  

### Requirement
```
conda install pytorch==1.7.0 torchvision==0.8.0 cudatoolkit=10.2 -c pytorch
```
See `requirements.txt` for additional dependencies and version requirements.
```setup
pip install -r requirements.txt
```

### Demo Test
Load the model in `--weights`

There are two testing methods.

#### Folder
Store the image or video in `--source`, and then save the result to `--save-dir`
```shell
python tools/demo.py --weights checkpoint.pth --source inference/images
```

#### Camera
For any camera connected to the computer, set the `source` as the camera number (the default is 0).
```
python tools/demo.py --weights checkpoint.pth --source 0 
```
