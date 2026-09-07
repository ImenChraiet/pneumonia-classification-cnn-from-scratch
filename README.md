# pneumonia-classification-CNN-from-scratch
Pneumonia classification from chest X-ray images using a Convolutional Neural Network (CNN) built entirely from scratch layer by layer, without using any pretrained models.

## Canvas Presentation link :
A presentation is included, providing a comprehensive journey through **Convolutional Neural Networks (CNNs)**:

- I did not just build a CNN and report an accuracy. I explained why I built it the way I did and why each choice was made.

- The presentation covers:

-**CNN Fundamentals:** An introduction to CNNs *from the ground up*, including the fundamental concepts behind convolutional neural networks, how they process images, and how they learn meaningful visual features.

-**Practical Project:** A complete walkthrough of applying these CNN concepts to **pneumonia detection using chest X-ray images**, connecting the theoretical concepts with the practical implementation.

-**CNN Architecture:** A detailed explanation of **every layer used in the CNN architecture**, including what each layer does, how it works, and *why it is included*. The architectural design choices are discussed and justified rather than simply presenting the final architecture.

-**Architectural Design Choices:** A step-by-step discussion of the decisions made when designing the CNN, including the choice and ordering of layers, feature extraction, pooling, normalization, activation functions, regularization, dropout, and the progression of the network throughout the architecture.

-**Training Configuration:** A detailed analysis of the **training settings and hyperparameters**, explaining the reasoning behind each choice rather than treating them as arbitrary values.

-**Optimization Algorithms:** An explanation of the different **optimizer algorithms**, their behavior, and how they differ in the way they update the model's weights. The presentation discusses the optimizers *in the order they were introduced in the literature*, analyzes their characteristics, and ultimately **justifies the choice of the optimizer used for the final model**.

-**Learning Rate Scheduling:** An explanation of the **learning rate**, its role during training, and the motivation behind using a **learning-rate scheduler**, including how dynamically adjusting the learning rate can influence the optimization process and model convergence.

-**Performance Analysis:** A discussion of the initial model's performance, the investigation into **class imbalance** as a potential factor affecting performance, and the subsequent improvement after balancing the classes, with accuracy increasing from **78% to 89%**.

> **From theory to practice:** The presentation does not simply present the final CNN model. It explains the **reasoning behind the decisions that led to it** — from understanding every architectural layer and its purpose, to selecting the optimizer and learning-rate strategy, and finally applying these choices to a real-world pneumonia classification problem.


## From Initial Model to Improved Performance (2 files)
The CNN was initially trained on the dataset **without addressing class imbalance**. The resulting model achieved only **78% accuracy**, which indicated that the model was not performing as expected.

Rather than immediately changing the CNN architecture, the model's performance and the dataset were investigated to identify the possible cause of the poor results. This analysis revealed a significant **class imbalance** in the dataset, which could cause the model to favor the majority class.

To address this issue, the classes were **balanced** and the CNN was retrained using the same *from-scratch* approach. After balancing the classes, the model's accuracy improved to **89%**.
> **Key insight:** Model performance is not determined solely by the architecture. Understanding the dataset and identifying issues such as **class imbalance** can be equally important.

## Acknowledgments

The dataset used in this project was obtained from the following Mendeley Data repository:

Labeled Optical Coherence Tomography (OCT) and Chest X-Ray Images for Classification

- Dataset: Mendeley Data (link : https://data.mendeley.com/datasets/rscbjbr9sj/2 )
- DOI: 10.17632/rscbjbr9sj.2
- Contributors: Daniel Kermany, Kang Zhang, and Michael Goldbaum
- License: CC BY 4.0
- Institutions: University of California San Diego

I acknowledge and thank the dataset contributors for making the data available for research and educational purposes.
