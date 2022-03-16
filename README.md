# Construction Machines Images Dataset

### Welcome to use and contribute to this dataset. we will highly appreciate your contribustions in building this open source dataset which would help lots of developers and researchers testing their work. Raw and prepocessed images data are all welcomed， as well as pretrained model. 
## The Goal
The main purpose of this repository is to construct an open source images dataset for construction machines detection. Due to the lack of data in this field, we aim, with the help of all contributer, to develop an intensive dataset that covers all type of construction machines and related objects to be used for research purposes.  As we initiate this repo, we have a relatively small dataset of excavators that was downloaded from google images search engine. The dataset consists of 223 image and their related label files in a YOLO format. Despite the low amount of images in this dataset, it still achives a pretty good performance when examined by training a YOLOv4 algorithm. However, This is just the first step towrdas building a comprehensive images dataset that contains as many classes of objects related to construction enviroments as possible. To get the job done, we are going to do our best to prepare data. Meanwhile, we are looking forward to having contribution from other developers and researchers.
Down below we will list some of the most important calsses that we can start with. To make things easy for other conributers, a work plan will be described below as well. 

### In case you would love to conribute to this dataset, please read the following: 
contribution to this dataset can be by upploading dataset of any of the object classes listed below. The data can be raw or prepocessed. In other words, you can upload raw images with no annotation files, also you are encourged to uplaod annotated images. In what follows, There are some tips for collecting and labeling the data.  
## Classes 
classes are all different kind of objects that someon would like to detect. In our case, as we are dealing with construction enviroments, the classes would be any object that may exists in a construction site. A list of some commonly related classes is as follows: 
1-excavators
2-trucks
3-bulldozers 
4-wheelloaders
5-cranes
7-backhow loaders
7-conctrete mixure trucks
8-graders
9-compactors
10-mobile cranes
11-tower cranes
12-workers , etc.

## Data collection 
The data can be collected in many ways: The hardest and the best way is to collect them manully by taking photos of different construction equipments from a constrcution site, this approach might be a bit difficult for many people. The second approach is to download images from the web either manull (one-by-one) of by using some web-mining techniques which are so popular online. The third approach is to capture photos from construction videos avialable online or taken by you previously. There might be approaches that dont come into my mind, feel free to use the one suits you. 

To ensure that the images collected are applicabe for model training, please pay attention to the following requirments: 
1-each images should at least contain one object class in it. 
2-the images should be of high resolution
3-the images must cover the whole outer view of the object
4-avoid images with small objects or those of far distance
5-avoid irregular images such as images that are taken in a dark light conditions or manipulated images
6-the images of the same object class should vary to cover a wide range of object positon , background , angles etc. 

Note: bad quality images have may cause negetive imapct on the trained model leading to bad accuracy in the predictions

## Data labeling 
After having the images prepared and filtered to meet the requirments，the images to be labeled so that when the dataset is fed into the algorithm for training the algorithm know what is in the images and starts leaning. There are many labeling tools avaiable online, some of them are open source while some other are commercial. A good exmaple of free open source labeling tools is labelImg tool where you can find it github repo [here](https://github.com/tzutalin/labelImg). Another great open-source labeling tool is called OpenLabeling the source code is availabel [here](https://github.com/techzizou/OpenLabeling), a useful tutorial on datasets labeling using OpenLabeling can be found in this [link](https://medium.com/analytics-vidhya/image-dataset-labeling-annotation-bec3390eda2d). Depending on what algorithm you intend to use to train you model, the label and annoutation format might differ. In our case we use YOLOv4, which require the labels to be in .txt files having the same name of the related images. If you use labelImg for labeling and bounding boxes annoutation, you can choose the format of the label file to be in YOLO format. One other thing to mension is that, make sure that you place the classes in a numbering order that does not change to avoid confusion when you set the configration for your YOLO algorithm. 

## Disclaimer 
Disclaimer: 
The data contained in this repository is downloaded from the google images search engine. This data is provided only for educational and research puposes. Some of the images might be copyrighted and use of them in any commercial application might require ask for permissions from the original creators. we strictly inform you that we are not the orginal producers of the images, but all of them have been webscraped for research purpose only. The label annotation files are created by us. 


