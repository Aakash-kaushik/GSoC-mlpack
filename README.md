![GSoC mlpack image](./assets/gsoc-mlpack.png)

**Organisation: [mlpack](https://github.com/mlpack)**

**Project: [Addition of ResNet Module and MobileNet V1](https://summerofcode.withgoogle.com/projects/#6085617844224000)**

**Mentors: [Marcus Edel](https://github.com/zoq) and [Kartik dutt](https://github.com/kartikdutt18)**

## Abstract

I was selected for google summer of code 2021 to work with mlpack on the project `Ready to use models in mlpack`, mlpack is an intuitive, fast, and flexible C++ machine learning library with bindings to other languages. In recent years computer vision has taken many turns and at this point, it is at a mature stage that when you need to use say a classification model you don't need to construct the complete architecture on your own, you can just write a single line of code and it creates the complete pretrained model for you which is what I did and added ResNet module and MobileNetV1 with pretrained weights on imagenet. 

## Goal

The goal of this proposal was to implement `MobileNetV1` which will also include implementing `depthwise separable convolutions` and a `ResNet` model builder that can be used to create `resnet18`, `resnet34`, `resnet50`, `resnet101`, and `resnet152`. This project would fall under the idea: `Ready to use models in mlpack`, the resnet builder and MobileNetV1 will fall under the [models](https://github.com/mlpack/models) repository and depthwise separable convolutions will fall under the mlpack repository as a layer inside the artificial neural network codebase.


## Results

Both the model builders that I proposed with pretrained weights with a lot of configuration are now available in the mlpack codebase. On the way, we faced and discovered small issues or implementation bugs which we corrected but we still face some issues with the tests of depthwise separable convolutions and so that PR is still not merged and before that, I would like to thank Kartik because yes the format I choose for writing this is originally his and yes this is 100% inspired by his with little tweaks of mine. 

## g++ Contributions.cpp -o Contributions

I have divided my contributions according to the repositories and PR having this ☀️ symbol in front of them was the core part of my projects others were mostly the ones that I picked up on the way but weren't mentioned in my project.

PS: The sun emoji because that resembles the GSoC logo. :p

### [mlpack/models](https://github.com/mlpack/models)

- [Addition of resnet module](https://github.com/mlpack/models/pull/63) - merged ☀️ 
- [Addition of MobileNet V1](https://github.com/mlpack/models/pull/72) - merged ☀️
- [Deprecation of ubuntu 16.04 in pipeline](https://github.com/mlpack/models/pull/67) - merged
- [Use catch2 instead of ctest](https://github.com/mlpack/models/pull/70) - merged
- [Ctest Fix](https://github.com/mlpack/models/pull/73) - merged
- [Documentation for models repo](https://github.com/mlpack/models/pull/65) - open

### [mlpack/mlpack](https://github.com/mlpack/mlpack)

- [Addition of DepthWise layer](https://github.com/mlpack/mlpack/pull/3007) - open ☀️
- [Documentation revamp](https://github.com/mlpack/mlpack/pull/2990) - open
- [Addition of ReLU6](https://github.com/mlpack/mlpack/pull/3009) - merged ☀️
- [Move Sequential layers to LayerTypes](https://github.com/mlpack/mlpack/pull/3004) - merged ☀️
- [Corrects wrong serialization for BatchNorm and Virtual BN](https://github.com/mlpack/mlpack/pull/2999) - merged ☀️
- [Padding layer fix for multiple filters](https://github.com/mlpack/mlpack/pull/2985) - merged ☀️

### [mlpack PyTorch Weight Translator](https://github.com/Aakash-kaushik/mlpack-PyTorch-Weight-Translator)

This repository was used to port weights for all the ResNet and MobileNetV1 from Pytorch and thus contains two branches, one for resnet and the other one for MobileNetV1.

- [Resnet](https://github.com/Aakash-kaushik/mlpack-PyTorch-Weight-Translator/tree/resnet)
- [MobileNet V1](https://github.com/Aakash-kaushik/mlpack-PyTorch-Weight-Translator/tree/mobilenetv1)

## Final Thoughts

I loved the time I spent with mlpack and would like to thanks my mentors Marcus and Kartik for guiding me with the best practices and helping me out whenever I was stuck. I would keep contributing to the project and the community as a whole with the things I have learned and would continue to learn.

## Ways to reach me

<p align="center">
  <a href="mailto:kaushikaakash7539@gmail.com?subject = Hello from your GitHub README&body = Message"><img src="./assets/gmail.svg" height="80px" width="80px" alt="Gmail" ></a>
  <a href="https://www.linkedin.com/in/kaushikaakash7539/"><img src="./assets/linkedIn.svg" height="80px" width="80px" alt="LinkedIn"></a>
</p>
