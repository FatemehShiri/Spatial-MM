# An Empirical Analysis on Spatial Reasoning Capabilities of Large Multimodal Models (EMNLP 2024)

Datasets for "An Empirical Analysis on Spatial Reasoning Capabilities of Large Multimodal Models". Our camera-ready copy is [here](https://aclanthology.org/2023.emnlp-main.568/). 


**Note:** Please feel free to leave a GitHub issue or shoot me an email at [fatimaa.shirii@gmail.com](mailto:fatimaa.shirii@gmail.com) if you have any questions about the data, or if you'd just like to chat about this (or related) work!

<p align="center">
<img src="figures/teaser.jpg" width="250">
</p>

Here's more information about the our benchmark, followed by instructions about how to use this repository to reproduce our results in the paper. 

# Benchmark
We introduce a novel benchmark, Spatial-MM, which includes two subsets: Spatial-Obj and Spatial-CoT. Spatial-Obj features multiple-choice questions that focus on the spatial relationships between one or two objects in an image, while Spatial-CoT offers
open-ended multi-hop questions.
Each subset is in a separate JSON file. The JSON files consist of the image ID and the list of answer options.


# Setting Up
Clone the repository and create the `data` directory within it, where your data and models will live. 
## Downloading the data
The data all lives in `spatial_mm/data`. 


You can also download the data directly from [this Google Drive link](https://drive.google.com/drive/u/3/folders/164q6X9hrvP-QYpi3ioSnfMuyHpG5oRkZ).

**Note:** As mentioned earlier, in all the datasets in our work (`Controlled_Images_A`, `Controlled_Images_B`, `COCO_QA_one_obj`, `COCO_QA_two_obj`, `VG_QA_one_obj`, `VG_QA_two_obj`), the first caption option is always the correct one. However, of the datasets that were already in the repository (`VG_Relation`, `VG_Attribution`, `COCO_Order`, `Flickr30k_Order`), in the first two of these, the second caption is correct, and in the next two of these, the first caption is correct. This is all handled by the evaluation code, so you don't have to worry about it; this is just for your reference, if you do choose to experiment with those datasets here (although I'd recommend switching back to the [original repository](https://github.com/mertyg/vision-language-models-are-bows)). 

## Running experiments with the models in the repo
This repository contains wrappers for several models (listed later in this section). You can run experiments with any of these models on any of the datasets in the repository to reproduce the paper results, or alternately write a wrapper for a new model and see how it does on our balanced spatial reasoning task. 


This will return the individual accuracy, as well as per-pair and per-set where applicable, i.e. the numbers in Table 3 of the paper. You can also run `marginalization.py` for the marginalization experiments in the paper (although they didn't yield much of an improvement). Table 1 in the paper reports macro-averages of subsets of each dataset: Controlled-A and Controlled-B, COCO/GQA one- and two-object. 



# Citation
If you use this code or data, please consider citing our paper:
```
@inproceedings{
  kamath2023whatsup,
  title={What's ``up'' with vision-language models? Investigating their struggle with spatial reasoning},
  author={Kamath, Amita and Hessel, Jack and Chang, Kai-Wei},
  booktitle={EMNLP},
  year={2024}
}
```
