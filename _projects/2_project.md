---
layout: page
title: Few-shot Learning for Energy Detection
description: a few-shot learning model to detect energy infrastructure (nuclear, solar, hydro) in aerial imagery.
img: assets/img/fewshot.png
importance: 1
category: academic
---
Abstract

Spatial images like GIS are large and can extend to several gigabytes. In addition, there are limited examples of energy infrastructure and it will be expensive to manually label the images. To mitigate this problem, we propose a few-shot setting-based energy infrastructure detection model that leverages embeddings trained on a smaller dataset. The main motivation of this project is to identify complex objects from the aerial imagery dataset. In this project, we implemented a few shot learning paradigm for unseen classes for energy infrastructure, namely nuclear power plant, solar photovoltaic power plant and conventional hydroelectric power plant.

We did some literature reviews on identifying complex objects from aerial imagery and chose two promising papers to follow up on their work on unseen object categories using few-shot learning. One is based on a regressing mechanism that detects the centre key points and then regresses the box boundary-aware vectors (BBAVectors). The other is based on an adaptive mechanism. Both of the chosen papers use the DOTA dataset which has 15 different classes excluding the dataset mentioned above. After reproducing the results for complex object detection from both papers, we use Protypical Networks to classify the unseen image classes. In the testing phase, we will use three-way three-shot learning to classify new classes not present in the training phase. The training strategy uses 3 different embeddings - two based on previously mentioned papers and another based on RESNET. These embeddings are used to train the model on three examples per unseen class and predictions will be made on new examples of the unseen classes.
