# YOLO_Streamlit
### Steps to run Code
1. Clone repo.
```
git clone https://github.com/Ericlinyuting/YOLO_Streamlit.git
```
- Goto the cloned folder.
```
cd YOLO_Streamlit

```
- Upgrade pip with mentioned command below.
```
pip install --upgrade pip
```

2. Install requirements.
- Install requirements with mentioned command below.
### Pip 
```
python3 -m venv .env
source .env/bin/activate
```
```
pip install Cython numpy(included in requirements.txt)(Optional)
```
```
pip install -r requirements.txt
```
- [Note]: `cython_bbox` have no windows distribution on pypi. If you're a windows user then run following command to install `cython_bbox` from source.
```
# for windows
pip install -e git+https://github.com/samson-wang/cython_bbox.git#egg=cython-bbox

# for linux
pip install cython-bbox
- Run the code with mentioned command below.


### conda
```
conda env create -f environment.yml
```
```
conda activate yolov7_bytetrack
```
- [Note]: `cython_bbox` have no windows distribution on pypi. If you're a windows user then run following command to install `cython_bbox` from source.
```
# for windows
pip install -e git+https://github.com/samson-wang/cython_bbox.git#egg=cython-bbox
# for linux
pip install cython-bbox

3. Download weights.
```
python download_weights.py
```

4. Run stremlit server
```
streamlit run yolov7-tiny-demo.py --server.port [LPORT]
```
- `LPORT` = Local port of system
### Test yolov7-tiny
- To run Yolov7-Tiny 
```
streamlit run yolov7-tiny-demo.py --server.port 2085
```
### Test yolov7
```
streamlit run yolov7-demo.py --server.port 2085
```
### Test yolor
```
streamlit run yolor-demo.py --server.port 2085
```
## Web app
Simple app consisting of a form where you can upload an image, and see the inference result of the model in the browser. Run:

`streamlit run yolov7-demo.py `

then visit http://localhost:8501 in your browser:

<p align="center">
<img src="https://github.com/noorkhokhar99/Object-Tracking-Dashboard-YOLOv7/blob/main/Screen%20Shot%201444-04-11%20at%2011.08.33%20PM.png">
</p>
