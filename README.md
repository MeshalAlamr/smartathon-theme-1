# SDAIA's Smartathon 2023 - Theme 1 - Team Pattrn


![img](https://user-images.githubusercontent.com/68873733/213890470-69f69f3a-0a07-4e7e-8791-d73b21a0f40a.png)

This project is a submission for SDAIA's Smartathon 2023, Theme 1. It aims to build a solution to detect and classify objects such as *graffiti, faded
signage, potholes, garbage, construction road,
broken signage, bad streetlight, bad billboard,
sand on road, clutter sidewalk, and unkept
facades.*



## Table of Contents

- [Main Notebook](#notebook)
- [Presentation](#presentation)
- [Technical Report](#report)
- [Perform Inference using Our Model](#start)
- [Model Weights](#model)
- [Authors](#authors)

## Main Notebook <a name="notebook" />
#### The main notebook details our complete work and how to replicate the training, and  adds more details on the inference. The notebook can be found [here](https://github.com/MeshalAlamr/smartathon-theme-1/blob/main/main.ipynb).

## Presentation <a name="presentation" />
#### The presentation showcasing an overview of the project and work can be found [here](https://github.com/MeshalAlamr/smartathon-theme-1/blob/main/presentation.pdf).

## Technical Report <a name="report" />
#### The technical report detailing the methodology and procedures can be found [here](https://github.com/MeshalAlamr/smartathon-theme-1/blob/main/report.pdf).

## Perform Inference using Our Model <a name="start" />
1. Clone this repository: <br>
```
git clone https://github.com/MeshalAlamr/smartathon-theme-1.git
```
2. Download the [Smartathon Theme 1 dataset](https://drive.google.com/file/d/1ULqYtd9yomeGz53WBhgRdPRFB37ppeDU/view) and unzip it in the root directory.

3. Install the project requirements:
```
cd smartathon-theme-1
pip install -r requirements.txt
```

4. To run the inference on the test.csv images of the contest using our model run the following:
```
python inference.py --model_name pattrn --segments 8
```
This will generate the output csv file containing the labels and bounding boxes for the visual pollutions in the ``results`` folder.

<b>Note</b>: In case you faced memory issues during inference, try to increase the ``segments`` parameter.


## Model Weights <a name="model" />
#### The final model weights can be found [here](https://github.com/MeshalAlamr/smartathon-theme-1/blob/main/models/pattrn/weights/best.pt).


## Authors <a name="authors"/>
- ### [Meshal Alamr](https://github.com/MeshalAlamr)
- ### [Abdulmajeed Almuarik](https://github.com/CreativeSelf0)
- ### [Saud Alrasheed](https://github.com/saudnr33)
- ### [Hussain Alkhayat](https://github.com/HussainAlkhayat)
- ### [Wael Mobeirek](https://github.com/waelmb)
- ### [Kumail Alhamoud](https://github.com/m1k2zoo)
