# Image-Caption-Generator


----
## Description
This repository contains files related to my project on Image Caption Generation.

----
## Dataset
1. Flickr30k Dataset has been used for the training of model.
   [Flickr30K](https://www.kaggle.com/hsankesara/flickr-image-dataset)
2. Glove6B dataset [Link](https://drive.google.com/open?id=1GI5sWeCxgJEgToeVmakL69oDlXowXGU4)
----
## Reference Paper
* Paper:[Show and Tell: A Neural Image Caption Generator](https://arxiv.org/pdf/1411.4555.pdf)
----
## Requirements
* Python 3.5
* Matplotlib
* Pandas
* Numpy
* PIL 
* Tkinter
* keras
* tensorflow

## Project Structure
----
   ├── beamsearch.py <br>
   ├── clean_captions.py<br>
   ├── Dataset<br>
   ├── Glove<br>
   │   └── glove.6B.300d.txt<br>
   ├── GreedyCaption.py<br>
   ├── app.py
   ├── ImageFeature_extraction.py<br>
   ├── images<br>
   │   ├── 101654506_8eb26cfb60.jpg<br>
   │   ├── 102455176_5f8ead62d5.jpg<br>
   │   ├── 106490881_5a2dd9b7bd.jpg<br>
   │   ├── 10815824_2997e03d76.jpg<br>
   │   ├── 20190908_182047.jpeg<br>
   │   ├── 20190908_185519.jpeg<br>
   │   ├── 47870024_73a4481f7d.jpg<br>
   │   ├── 56494233_1824005879.jpg<br>
   │   └── pic.jpeg<br>
   ├── index.jpeg<br>
   ├── model_weights<br>
   │   └── FinalModel.h5<br>
   ├── Preprocessed Data<br>
   │   ├── clean_captions.pkl<br>
   │   ├── Image_features.pkl<br>
   │   └── vocabulary.pkl<br>
   ├── requirements.txt<br>
   ├── training.py<br>
   └── vocabulary.py<br>

## Model flow Chart
----
<img src="https://github.com/udaram/Image-Caption-Generator/blob/master/model.png">

 ##install python latest version with libraries mentioned in requirements   ```
## Run Model in steps
##first open the folder in terminal
---
*Image Feature Extraction*
--------------------------
```
$ python3 ImageFeature_extraction.py
```
*Caption Preprocessing step*
--------------------------
```
$ python3 clean_captions.py
```
*Generating Vocabulary of Caption words*
--------------------------
```
$ python3 vocabulary.py
```
*Training of the Model*
--------------------------
```
$ python3 training.py
```
*Test model*
--------------------------
```
$ python3 app.py

this gui is made using python Tkinter package 
```

## Testing The Model
---


```### interface result
command:-
     python -m flask run


