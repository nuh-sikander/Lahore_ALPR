You need to setup the follwing on windows and place the **detention_all.py** file in the yolov5 folder

```bash
git clone https://github.com/ultralytics/yolov5 # clone repo
python3 -c "from yolov5.utils.google_utils import gdrive_download; gdrive_download('1n_oKgR81BJtqk75b00eAjdv03qVCQn2f','coco128.zip')" # download dataset
cd yolov5
pip install -U -r requirements.txt
```
## Fixes for issues with Windows install
Having issues with installing under Windows? Try the following.
```bash
pip install torch==1.5.1+cpu torchvision==0.6.1+cpu -f https://download.pytorch.org/whl/torch_stable.html
pip install "git+https://github.com/philferriere/cocoapi.git#egg=pycocotools&subdirectory=PythonAPI"
pip install git+https://github.com/philferriere/cocoapi.git#subdirectory=PythonAPI
```
