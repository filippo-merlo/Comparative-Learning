# Human Inspired Progressive Alignment and Comparative Learning for Grounded Word Acquisition

## Abstract
Human language acquisition is an efficient, supervised, and continual process. In this work, we took inspiration from how human babies acquire their first language, and developed a computational process for word acquisition through comparative learning. Motivated by cognitive findings, we generated a small dataset that enables the computation models to compare the similarities and differences of various attributes, learn to filter out and extract the common information for each shared linguistic label. We frame the acquisition of words as not only the information filtration process, but also as representation-symbol mapping. This procedure does not involve a fixed vocabulary size, nor a discriminative objective, and allows the models to continually learn more concepts efficiently. Our results in controlled experiments have shown the potential of this approach for efficient continual learning of grounded words.


## [Dataset] **SOLA**: **S**imulated **O**bjects for **L**anguage **A**cquisition

**SOLA (Simulated Objects for Language Acquisition)** is a small clean dataset with little noise and clearly defined attributes for efficient comparative learning and grounded language acquisition. It is generated using the open\-source simulation software [Kubric](https://github.com/google-research/kubric).

![alt text](https://github.com/sled-group/Comparative-Learning/blob/main/assets/dataset_figure.png)


### Dataset Stats

|Learning Attributes  |Changing Attributes |Variation Attributes |
| ------------- | ------------- | ------------- |
| Color: 8 | Lighting: 3  | Shade: 3 |
| Material: 4  | Camera Angle: 6  | Size: 3 |
| Shape: 11 | |Stretch: 4|
|**Total:**| **6336 (RBGA)** | **989 (RGBA)**|


**Image Types (5):** RGBA, Depth, Surface Normal, Segmentation Map, Object Coordinates


### Dataset Download

Dropbox Link: [LINK](https://www.dropbox.com/sh/irnw2jdw3vs9od9/AACB1SqQWeWE7hjJTfhTRhA5a?dl=0)
Hugging Face: [LINK](https://huggingface.co/datasets/sled-umich/SOLA)


## [Method] **Comparative Learning**