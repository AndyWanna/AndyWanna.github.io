---
layout: page
title: Machine and Deep Learning Projects
description: Predicting House Value - NN Regression Project, Medical MRI Scans - CNN Computer Vision Project
img: assets/img/ML/viz.jpg
importance: 3
category: Software
---

Here are both my ML/DL projects.

The first was creating a classic Neural Network with PyTorch to predict the value of a house in San Francisco, based on its input formation. This involved data-preprocessing, constructing the NN in PyTorch and evalutaing hyper parameters such as network shape and gradient descent algorithim via k-cross-folds hyperparameter tuning. 

The second project was a computer vision task and required implementing a U-Net Convolutional Neural Network architecture in PyTorch, to automatically detect potential cancerous regions in brain MRI scan. This project focused more on implemnting the convolutional pass-through and feedback architecture, along with using performance metrics to accurately evaluate the quality of our model.


<div class="row justify-content-sm-center">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/ML/viz.jpg" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm mt-3 mt-md-0">
        <video>
            {% include figure.html path="assets/img/ML/ML-CW2.png" title="example image" class="img-fluid rounded z-depth-1" %}
        </video>
    </div>
</div>
<div class="caption">
    Left: Predicted versus ground-truth results for brain MRI scans. Right: Performance of NN Model on both train and validation sets to determine ideal epochs.
</div>
