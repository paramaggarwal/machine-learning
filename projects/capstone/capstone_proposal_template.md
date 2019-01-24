# Machine Learning Engineer Nanodegree
## Capstone Proposal
Param Aggarwal 
January 24th, 2019

## Proposal

### Domain Background

Myntra is a fashion e-commerce company in India that has a very large catalog of products to choose from. One can use their website or app to browse through products and buy them. This catalog is manually photographed and uploaded into the Content Management System (CMS). This presents a challenge regarding the validity of this data. Often incorrect images are uploaded and have to be manually verified and removed from the catalog before publishing to the main website.

I have been an employee of Myntra and have seen these problems first hand. My motivation to resolve this issue comes from the understanding of how much such a system could be useful to the company.

### Problem Statement

As of today this approach involves a lot of stages of manual review and approval. This increases the time from when an item is photographed to when it goes live on the website and can contribute to lost revenue. Fashion is a fast moving industry and new trends have to hit the market as soon as possible. Any attempts at speeding up the review process can help directly contribute to an increase in revenue.

### Datasets and Inputs

The dataset is downloaded from the Myntra website for existing products that are listed. Hence we also have the labels for these images. For example we know whether the item is a 'topwear' or 'bottomwear'. The dataset consists of 2000 images with half and half split between topwear and bottomwear.

These images are in jpeg format in a suitable resolution with the product identifier as the filename. We also have a separate JSON file which contains the attributes of the image, for example, the category of the clothing. This will be used as labels for our supervised machine learning.

### Solution Statement

We will be training a Convolutional Neural Network supervised using the category labels in our dataset. We will be using Keras for this and will be using the `accuracy` score as the metric or optimizing our network.

### Benchmark Model

As of today this verification is a manual approach. Hence the accuracy of a random classifier will be `0.5` or 50%. Our aim in building our neural network classifier is to beat this benchmark.

### Evaluation Metrics

We will be evaluating our network performance by splitting out around 20% of our data to be used as a test set. The `accuracy` score obtained on this dataset will be our evaluation metric. As mentioned above, our goal is to beat the 50% accuracy that a random classifier might have.

### Project Design

We need to go through our data once and check that the downloaded dataset images are not corrupted. We will then build our Keras model layers step by step and come up with a Convolutional Neural Network that is trained with the category labels as the supervised learning parameters.

Once we are done with this, we will use some random images from the website to simulate how the system would work for verification of newly uploaded images and point out errors that would be caught before the product goes live on the website.

