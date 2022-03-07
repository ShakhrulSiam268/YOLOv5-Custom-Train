## Dataset Structure

```
 ├── YOLOv5-Custom-Train
 └── datasets
     └── dataset_name
        └── images
        └── labels
```

If you want to follow different folder structure, update Dataset Directory path in `./data/dataset_name.yaml` file.


## Training
Run 

`python train.py --img 640 --batch 8 --epochs 50 --data dataset_name.yaml --weights ./model_data/yolov5s.pt`

use smaller batch size to prevent GPU Memory exceed error.

Model and Results will be saved at `run/train/exp*` folder as 
`best.pt` and `last.pt`.
