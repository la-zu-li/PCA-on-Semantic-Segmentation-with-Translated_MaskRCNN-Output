# PCA-on-Semantic-Segmentation-with-Translated_MaskRCNN-Output

PCA to calculate longest diagonal of C3S crystals of semantic segmentation from an implementation of MaskRCNN.

## About

This repository is for an academic research in Federal University of Ceará, Campus Russas, Brazil.
It features the application of the PCA (Principal Component Analysis) algorithm on the masks of C3S crystals, segmented by an architecture of mask-RCNN. This repository contains code for the use of a specific architecture of mask-RCNN implemented with Tensorflow2.

## The research

The measurement of C3S crystals is an important part of a stage of portland cement production, the clynker microscopy. It is mostly done by analysts, by examinating microscopic images of the clynker (a subproduct of cement) and measuring the crystals manually, in computers, with the help of drawing software. The research is about automating this, and there's where the PCA algorithm enters.

The algorithm showed good approximated results for the longest diagonal of the polygons segmented by the network of the C3S crystals, and a very good performance. This repository aims to show these results.

### The network

The Mask-RCNN architecture used was implemented with Tensorflow and migrated to Tensorflow 2.8 and enhanced by Renê Michel. It is also part of the research, which also includes a comparative analysis of this architecture and another from Detectron2 API.

You can find Michel's code for it in [this repository](https://github.com/Rene-Michel99/Mask-RCNN-TF2.8.git).

Also, you can find the alternative code for Detectron2 on [this repository](https://github.com/la-zu-li/PCA-on-Semantic-Segmentation-with-Detectron2).

## Contents

This repository contains two python notebooks:

- *PCA_with_Translated_Mask_Output.ipynb*;
- *PCA_with_Translated_Mask_Output_COLAB.ipynb*

Plus the folder '*pretrained_weights/*'.

The first noteboook is in case you want to clone this repository and run it in your computer.
The second notebook is for running in Google Colab environment.

The '*pretrained_weights/*' folder contains the pre-trained weights. They are needed so that we don't need to go through the process of training the network again. The weights are loaded by the network, which makes it ready for inference.

## Running in your machine

When running in your machine, use the *'PCA_with_Translated_Mask_Output.ipynb'* notebook. The other one will only work in colab.

There's code in the notebook for installing missing libraries via `pip`, so make sure to have it installed and well-updated.

After opening the notebook with a software from your choice, just run all cells in sequence.

## Running in Google Colab

When running in Colab, use the notebook *'PCA_with_Translated_Mask_Output_COLAB.ipynb'*. The other one will not work properly there.
It's very recommended to run in Google Colab with GPU hardware accelerator. The GPU helps accelerating the inference process.

After opening the notebook in Colab, run all cells in sequence.