# ship tracking

SORT is a tracking method based on a detection model and the kalman filter. In this Github we use a pretrained yolov3 (we can also use yolov5).

## Setup


The first step is to set up the environment.
```sh
# set the environment
conda env create -f trackenv.yml
conda activate 
```
We can use the sort model with any detection model. to use it with the yolov3:

```sh
#download the yolov3 weight"
wget https://pjreddie.com/media/files/yolov3.weights
```
Change the video path on track.py
//
Then use the SORT algorithm on the output video.

```sh
python track.py
```
