## Weakly Supervised Learning Guided by Activation Mapping Applied to a Novel Citrus Pest Benchmark

This project contains the source code described in 'Weakly supervised learning guided by activation mapping applied to a novel citrus pest benchmark.' This [work](https://arxiv.org/pdf/2004.11252.pdf) was published in Agriculture-Vision Workshop @ CVPR 2020.

This code is an example of how to use Grad-CAM to produce instances for a multiple instance learning method. It uses the [Citrus Pest Benchmark](https://github.com/edsonbollis/Citrus-Pest-Benchmark) in the training process. The weakly supervised multi-instance learning code presents a way to classify tiny regions of interest (ROIs) through a convolutional neural network, a selection strategy based on saliency maps, and a weighted evaluation method.

![Mite Images](https://github.com/edsonbollis/Weakly-Supervised-Learning-Citrus-Pest-Benchmark/blob/master/pipeline_transfer_learning.png)

Our method consists of four steps. In Step 1, we train a CNN (initially trained on the ImageNet) on the Citrus
Pest Benchmark. In Step 2, we automatically generate multiple patches regarding saliency maps. In Step 3, we fine-tune our
CNN model (trained on the target task) according to a multiple instance learning approach. In Step 4, we apply a weighted
evaluation scheme to predict the image class.


### Citation
```
@inproceedings{bollis2020weakly,
  title     = {Weakly Supervised Learning Guided by Activation Mapping Applied to a Novel Citrus Pest Benchmark},
  author    = {Edson Bollis and Helio Pedrini and Sandra Avila},
  booktitle = {{IEEE} Conference on Computer Vision and Pattern Recognition Workshops (CVPRW)},
  year      = {2020}
}
```

### Acknowledgments
E. Bollis is partially funded by CAPES (88882.329130/2019-01). H. Pedrini is partially funded by FAPESP (2014/12236-1, 2017/12646-3) and CNPq (309330/2018-1). S. Avila is partially funded by FAPESP (2013/08293-7, 2017/16246-0) and Google Research Awards for Latin America 2019. RECOD Lab. is partially supported by diverse projects and grants from FAPESP, CNPq, and CAPES. We gratefully acknowledge the donation of GPUs by NVIDIA Corporation.

ATTN: This code is free for academic usage. For other purposes, please contact Edson Bollis (edsonbollis@gmail.com).
