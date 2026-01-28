# Diffusion Noise Feature: Accurate and Fast Generated Image Detection

[Yichi Zhang](https://yichics.github.io/) and [Xiaogang Xu](https://xiaogang00.github.io/)

Code repository for the paper: [Diffusion Noise Feature: Accurate and Fast Generated Image Detection](https://arxiv.org/abs/2312.02625v2). 

![fig](fig/fig1.png)

### Baseline

The code is based on [CNNDetction](https://github.com/PeterWang512/CNNDetection)


**Model Preparation**

The new checkpoints will release soon.

Download the LSUN Bedroom pretrained DDIM from [here](https://heibox.uni-heidelberg.de/f/f179d4f21ebc4d43bbfe/?dl=1). Place it in `./weights/diffusion/` .

**Dataset Preparation**

The testsets can be download from [Huggingface](https://huggingface.co/datasets/toru0035/DNFTestSet).
Download the **DiffusionForensics** from  [DIRE](https://github.com/ZhendongWang6/DIRE). 

Please refer to [CNNDetction](https://github.com/PeterWang512/CNNDetection) for the storage path of the dataset.

**Transform Image to DNF**

```
python compute_dnf.py
```

**Training**

```
python train.py 
```
**Evaluation**

```
python eval.py 
```


Please refer to `./options` for variables that determine the program’s execution.


### Citation 

```
@inbook{zhang2025diffusion,
  title = {Diffusion Noise Feature: Accurate and Fast Generated Image Detection},
  ISBN = {9781643686318},
  ISSN = {1879-8314},
  url = {http://dx.doi.org/10.3233/FAIA250925},
  DOI = {10.3233/faia250925},
  booktitle = {ECAI 2025},
  publisher = {IOS Press},
  author = {Zhang,  Yichi and Xu,  Xiaogang},
  year = {2025},
  month = oct 
}
```
