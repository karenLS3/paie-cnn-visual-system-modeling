# Project title: Convolutional neuronal network as a model for object recognition in the visual system

> [PAIE - CSIC](https://www.estudiantes.csic.edu.uy/) - [UdelaR](https://udelar.edu.uy/portal/) - [UTEC](https://utec.edu.uy/en/)

This project is an introductory undergraduate research initiative, designed to familiarize the team with key concepts in neuroscience and artificial neural networks. It focuses on investigating how selectivity and invariance evolve across the layers of a convolutional neural network (CNN), drawing inspiration from the experiments conducted by Rust and DiCarlo (2010) on visual information processing in macaque monkeys. By replicating these experiments and comparing the results with the behavior of CNNs, the project aims to deepen our understanding of how visual features are encoded and transformed, contributing to a broader insight into object recognition in biological and artificial systems.

## Method

We use a pre-trained CNN on an image classification task to record its neural activations. By analyzing how these activations change in response to various input image transformations, we can compare these changes with those observed in the macaque brain.

1. **CNN Selection and Preparation:** we will search for and download an existing open-access CNN trained for the image classification task. Then, since AI models typically do not record their neural activations, we will modify the architecture to add a program that records these activations.
2. **Dataset Generation:** Using an image editing program, we will replicate the manipulations from Rust and DiCarlo (2010) (e.g., variations in size, object position, and texture).
3. **Image Presentation and Data Collection:** The generated images, including altered images, are presented to the CNN. We save the neural activations for analysis.
4. **Analysis:** Statistical methods, based on those in Rust and DiCarlo's article, will be used to quantify selectivity and invariance across neural layers.
5. **Comparison of Results:** We will assess the robustness of these identified groups, for example, by comparing the results obtained with the machine learning method to an analysis that measures the distance between neural activations for different images, as conducted in Rust and DiCarlo (2010).

## Project Overview

The complete investigation can be found in the following notebook: [CNN_PAIE_Project.ipynb](src/CNN_PAIE_Project.ipynb).

### Image Sources

The images used in this project were sourced from:
* **squirrel.png** from user Cristian Martinez on [Flickr](https://www.flickr.com/photos/cfuga/445759644)
* **termo.png** from user Wirestock on [Freepik](https://www.freepik.com/free-photo/vertical-closeup-cup-yerba-mate-infusion-with-thermos_23835560.htm#fromView=search&page=1&position=16&uuid=43a6a496-2133-4c71-b008-5848155c4c5d)

### Technologies Used

* Python
* PyTorch
* Jupyter Notebook
* Matplotlib

### Team Members

* Rocío Lión
* Micaela De Mori
* Karen Lima @karenLS23 :elf:

### Advisor

* Daniel Herrera (Neuroscience Lab)


# References
<a id="1">[1]</a>
Rust, N. C., & DiCarlo, J. J. (2010). Selectivity and Tolerance (“Invariance”) Both Increase as Visual Information Propagates from Cortical Area V4 to IT. Journal of Neuroscience, 30(39), 12978–12995. https://doi.org/10.1523/jneurosci.0179-10.2010

<a id="2">[2]</a>
Simonyan, K., & Zisserman, A. (2014). Very deep convolutional networks for large-scale image recognition. arXiv preprint arXiv:1409.1556.

<a id="3">[3]</a>
Vinje, W. E., & Gallant, J. L. (2000). Sparse Coding and Decorrelation in Primary Visual Cortex During Natural Vision. Science, 287(5456), 1273-1276.

<a id="4">[4]</a>
Rust, N. C., and J. J. DiCarlo. “Balanced Increases in Selectivity and Tolerance Produce Constant Sparseness Along the Ventral Visual Stream.” Journal of Neuroscience 32.30 (2012): 10170–10182.