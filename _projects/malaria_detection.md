---
layout: page
title: Malaria Parasite Detection
description: Designing CNN architectures for high-accuracy detection.
img: /assets/img/malaria.jpg
importance: 1
category: work
related_publications: false
---

## Project Overview
This project focuses on **Bio-Computing** by applying deep learning techniques to medical imaging. The goal was to automate the detection of malaria parasites in blood smear images to assist healthcare professionals.

### Key Features
* **Architecture**: Designed a custom Convolutional Neural Network (CNN) specifically for high-resolution cell images.
* **Accuracy**: Achieved high accuracy on the test set, outperforming standard baseline models.
* **Dataset**: Utilized the publicly available **NIH Malaria Dataset**.

### Technical Details
* **Frameworks**: Implemented using **PyTorch** for model development and training.
* **Optimization**: Utilized **transfer learning** to optimize training time and improve convergence on the limited dataset.
* **Preprocessing**: Applied image augmentation techniques (rotation, flipping, normalization) to increase model robustness.

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/publication_preview/malaria.jpg" title="Malaria Cell Image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    Sample output showing detected parasite cells.
</div>
