# EfficientDet-Object-Detection
PyTorch Implementation of EfficientDet: Scalable and Efficient Object Detection **EfficientDet: Scalable and Efficient Object Detection** [paper](https://arxiv.org/abs/1911.09070)

To run object Detection on Google Colab - 

https://colab.research.google.com/drive/1dugPLJDZJLFhya9pcdU-gk1d7YrzZJQp?usp=sharing

NOTE: Upload your video in the "Test_Videos" folder and the detected output video will be saved in "output_folder" you can download it later

Create a data folder under the repository,

```
cd {repo_root}
mkdir data
```
  
- **COCO**:
  Download the coco images and annotations from [coco website](http://cocodataset.org/#download). Make sure to put the files as the following structure:
  ```
  COCO
  ├── annotations
  │   ├── instances_train2017.json
  │   └── instances_val2017.json
  │── images
      ├── train2017
      └── val2017
  ```
* **Train your model** by running **python train.py**
* **Evaluate mAP for COCO dataset** by running **python mAP_evaluation.py**
* **Test your model for COCO dataset** by running **python test_dataset.py --pretrained_model path/to/trained_model**
* **Test your model for video** by running **python test_video.py --pretrained_model path/to/trained_model --input path/to/input/file --output path/to/output/file**

