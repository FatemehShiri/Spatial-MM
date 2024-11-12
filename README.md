# An Empirical Analysis on Spatial Reasoning Capabilities of Large Multimodal Models (EMNLP 2024)

Datasets for "An Empirical Analysis on Spatial Reasoning Capabilities of Large Multimodal Models". Our camera-ready copy is [here](https://arxiv.org/submit/5988550). 


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


You can also download the data directly from [this Google Drive link](https://drive.google.com/drive/folders/17J2nFEDS0_Jc9MIyQksA2ENFyxmJk0B2?usp=sharing).



# Citation
If you use this code or data, please consider citing our paper:
```
@inproceedings{shiri2024empirical,
  title={An Empirical Analysis on Spatial Reasoning Capabilities of Large Multimodal Models},
  author={Shiri, Fatemeh and Guo, Xiao-Yu and Far, Mona and Yu, Xin and Haf, Reza and Li, Yuan-Fang},
  booktitle={Proceedings of the 2024 Conference on Empirical Methods in Natural Language Processing},
  pages={21440--21455},
  year={2024}
}
```
