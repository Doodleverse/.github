# :space_invader: Welcome to the Doodleverse :space_invader:

[![Gitter chat](https://badges.gitter.im/Doodleverse.png)](https://gitter.im/doodleverse)

The doodleverse is an opinionated collection of Python packages designed for geoscientific image segmentation.  

<!-- ![](https://user-images.githubusercontent.com/3596509/153691058-fd1d0af0-03ba-49fe-9dbe-1007f700e006.png) -->

![doodleverse3_blackborder](https://user-images.githubusercontent.com/3596509/153729377-e16d0679-ca0d-4d0d-a9f9-90306ba2f871.png)

## ✍️ Authors

Package maintainers:
* [@dbuscombe-usgs](https://github.com/dbuscombe-usgs) 
* [@ebgoldstein](https://github.com/ebgoldstein)

## 🌟 Overview
Currently, there are 3 packages:

### Dash-Doodler
![](https://github.com/Doodleverse/dash_doodler/blob/main/doodler-logo.png)

  * For fast, interactive segmentation of imagery
  * For creation of training datasets for training Machine-Learning-based image segmentation models, for example Segmentation Gym

### Segmentation Gym
<!-- ![zoo](https://user-images.githubusercontent.com/3596509/153691733-1fe98e37-5379-4122-8d02-adbcb0ab0db3.png) -->
![gym](https://user-images.githubusercontent.com/3596509/153696396-0b3148c5-77e4-48b2-b3ce-fd9038ba21ab.png)

  * A neural gym for training image segmentation models based on fully convolutional models based on UNets
  * This repository is where you train models based on your own imagery and label data, and evaluate those models

### Segmentation Zoo
![zoo](https://user-images.githubusercontent.com/3596509/153691807-1da4d3ba-377b-40af-9891-c469cc6390c1.png)

  * A repository of pre-trained Gym models for some common tasks
  * A set of notebooks that illustrate how best to use a model on sample imagery
  * You are encouraged to contribute your Gym models for the common good!

Packages are compatible, and share an underlying design and data structures


## 💨 Applications and datasets built on top of Doodler, Gym, and Zoo

### Holo-Doodler

  * A port of Dash-Doodler using the Anaconda/Holoviews API for graphical user interface
  * Dash-Doodler and Holo-Doodler both use the same codes for image label generation, found in `doodler_engine` repo

### Seg2Map
![](https://user-images.githubusercontent.com/3596509/194389595-82ade668-daf0-4d24-b1a0-6ecf897f40fe.gif)

  * A mapping extension for application of Segmentation Zoo models on geospatial imagery
  * Uses codes housed in [s2mengine](https://github.com/Doodleverse/s2m_engine) for conversion of label images (from Gym and Doodler) into geospatial formats, and for visualization of generic label images in geospatial formats in a small webGIS viewer

### CoastSeg
![](https://user-images.githubusercontent.com/3596509/189417290-d5c24681-39b7-4b97-afa8-1392cf759b08.gif)

  * A mapping extension for [CoastSat](https://github.com/kvos/CoastSat) using Segmentation Zoo models
  * Provides a graphical browser-based environment for application of the CoastSat workflow for shoreline mapping
  * Provides a graphical browser-based environment for application of Segmentation Zoo models for mapping features in satellite imagery

### Coast Train
![](https://github.com/CoastTrain/CoastTrain/raw/main/website/static/img/Coast_train_fig1.jpg)

  * Coast Train is a dataset made using Doodler, and has been used for training Zoo models that are being implemented in CoastSeg, Seg2Map, and elsewhere
  * The Coast Train repo is [here](https://github.com/CoastTrain/CoastTrain)
  * Consult the Coast Train [website](https://coasttrain.github.io/CoastTrain/) for more info. Data may be accessed from [here](https://coasttrain.github.io/CoastTrain/docs/Version%201:%20March%202022/data)


## What is opinionated software?

Opinionated Software is a software product that encodes a specific way of approaching a task. The Doodleverse is a well-researched end-to-end data-model pipeline for geoscientific image segmentation that has a lot of practices baked into it. In particular, the Doodleverse implements a specific data-creation and model-training pipeline. See [this link](https://medium.com/@stueccles/the-rise-of-opinionated-software-ca1ba0140d5b#.etoe6fbd2) and [this article](https://peerj.com/preprints/3210/) for more reading around this topic.






