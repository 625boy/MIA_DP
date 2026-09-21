## MIA_DP
This repository contains experiments for evaluating privacy leakage in deep neural networks using Membership Inference Attacks (MIA) and investigating the effect of Differential Privacy (DP) on model privacy and utility.

## Dataset
The experiments are based on a ResNet18 image classifier trained on CIFAR-10.

The datasets are automatically downloaded through `torchvision` when running the notebooks.

## Experiments
# Membership Inference Attack
`MIA_result.ipynb` contains experiments for evaluating privacy leakage of the pre-trained model.
# Differential Privacy
`DP_result.ipynb` applies Differential Privacy using `Opacus` and evaluates the resulting privacy–utility trade-off.

The notebook considers different DP training strategies, including:
* Full-model DP training
* Partial-layer DP training
* Final-layer DP training

The experiments evaluate:
* Test accuracy
* Privacy budget
* MIA AUC

## Directory and Codes
```
.
+-- train_model
|       +-- models
|       |      +-- __init__.py
|       |      +-- resnet_test.py
|       +-- main.py
|       +-- utils.py
+-- notebooks
|       +-- DP_result.ipynb
|       +-- MIA_result.ipynb
+-- modules 
|       +-- figure_diff_dp.png
|       +-- figure_diff_mia.png
|       +-- figure_label.png
|       +-- figure_mia.png
|       +-- figure_roc.png
|       +-- figure_test.png
|       +-- figure_train.png
+-- LICENSE
+-- README.md
```

## Acknowledgement
이 논문은 정부(과학기술정보통신부)의 재원으로 한국연구재단의 지원을 받아 수행된 연구임 (NO. RS-2022-NR068754)

This research was supported by the National Research Foundation of Korea(NRF) grant funded by the Korea government(MSIT) (NO. RS-2022-NR068754)
