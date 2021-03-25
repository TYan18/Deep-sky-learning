## Project: Deep Sky Learning

This repository contains a description and the files relevant to this deep learning project.

## Goal

The goal of this project is to access the publically available data stored in the Dark Energy Survey, and correctly classify images containing supernovae taken by powerful telescopes, using a convolutional neural network (CNN) deep learning technique.

## Description

Since Einstein's famous general theory of relativity, and Edwin Hubble's observations that the universe appears to be expanding, there has been much speculation in the field of astronomy, astrophysics, and cosmology about the existence of a mysterious force driving this expansion. It is now believed that approximately 70% of the combined mass and energy in the universe resides in this mysterious force, which has been called dark energy.

Not much is known about dark energy, but one way to indirectly study it involves examining a special type of supernova, called Type Ia. A supernova is an explosion of a heavy star after it finally burns through its nuclear fusion fuel source. Type Ia supernovae have a characteristic brightness depending on how far away they are, and their observed brightness gives insights into the expanding distance in between. However, they are not always apparent within a telescopic image.

Up until recently, astronomers didn't have much choice but to manually look through images to determine which ones contained this type of supernovae. With deep learning and CNN algorithms, this project aims to build a classifier to help astronomers save time by automatically identifying these supernovae.

## What's in this repo

This repo contains a pickled dataset of images and labels from the 2013-2014 observing season of the Dark Energy Survey, originally extracted from the [Autoscan project](https://portal.nersc.gov/project/dessn/autoscan/). Further data can be found directly from this website. Here, only the data from 2014 is provided.

The file "CNN_classifier.ipynb" contains the code for unpickling and fitting the data to a simple CNN model architecture. It shows that although the accuracy, precision, and recall were subpar in the simple model, large increases in these performance metrics were obtained by applying a transfer learning method.

## Acknowledgements

1. [Space2Vec](http://space2vec.com/): Project inspiration, prior work on CNN classification model for supernova in telescope images
2. [Autoscan](https://portal.nersc.gov/project/dessn/autoscan/): Labelled image dataset, prior work on detecting supernova with machine learning via random forest model
3. [Astropy](https://www.astropy.org/): Package for handling .fits image data files in Python