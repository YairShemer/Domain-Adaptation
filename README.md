# Domain-Adaptation

## Papers
* [Ship classification from overhead imagery using synthetic data and domain adaptation (2019)](https://arxiv.org/pdf/1905.03894.pdf)
  * Building a large (200k) dataset of synthetic ships and using it to increase classification performance with domain adaptation
* [Unsupervised Domain Adaptation by Backpropagation (2015)](https://arxiv.org/pdf/1409.7495.pdf)  
  * Train a NN to discriminate between different classes while being invariant with respect to the shift between the domains.
  * Simple and easy to implement.
  * This paper was extended by a following paper of the same author: [Domain-Adversarial Training of Neural Networks (2016)](https://arxiv.org/pdf/1505.07818.pdf)
* [Unsupervised Pixel-Level Domain Adaptation With Generative Adversarial Networks (2017)](http://openaccess.thecvf.com/content_cvpr_2017/html/Bousmalis_Unsupervised_Pixel-Level_Domain_CVPR_2017_paper.html)  
  * [CVPR 2017 oral](https://www.youtube.com/watch?v=VhsTrWPvjcA)
* [Maximum Classifier Discrepancy for Unsupervised Domain Adaptation](http://openaccess.thecvf.com/content_cvpr_2018/papers/Saito_Maximum_Classifier_Discrepancy_CVPR_2018_paper.pdf)  
  * Train two different classifiers for the source while maximizing the discrepancy between them. Meanwhile, train the feature generator to minimize the discrepancy. 
  * [Code](https://github.com/mil-tokyo/MCD_DA/tree/master/classification)
   * [CVPR 2018 oral](https://www.youtube.com/watch?v=8mk7i3vGjAM)
* [Unsupervised Domain Adaptation with Similarity Learning (CVPR 2018)](https://openaccess.thecvf.com/content_cvpr_2018/papers/Pinheiro_Unsupervised_Domain_Adaptation_CVPR_2018_paper.pdf)  
  * Train two different networkes: 1. Generate features that are domain invariant (and also good for the similarity operation mensioned below). 2. Generate features that the similarity between them and the first features indicates the classes. 
  * Show good results on images generated from CAD models.
  * What is the advantage of this method compared to the calssic advarsial approach?
* [Deep CORAL: Correlation Alignment for Deep Domain Adaptation (2016)](https://arxiv.org/pdf/1607.01719.pdf)
  * Minimize a CORAL loss, i.e. minimize the difference between the second moment of the source feautres and the second moment of the target features.
* [Learning from Synthetic Animals (CVPR 2020)](https://arxiv.org/pdf/1912.08265.pdf)
  * Generate Pseudo-Labels by iteratively apply the current model and check the consistencies of it.
  * Augment the synthetic data - "An animal with random poses and random texture is rendered from a random viewpoint for some random lighting
and a random background image."
* [Contrastive Adaptation Network for Unsupervised Domain Adaptation (CVPR 2019)](https://openaccess.thecvf.com/content_CVPR_2019/papers/Kang_Contrastive_Adaptation_Network_for_Unsupervised_Domain_Adaptation_CVPR_2019_paper.pdf)
  * State-of-the-art results on office-31 dataset (90.6%) and visDA2017 (87.2%, 10% above the second!).
* [Learning Transferable Features with Deep Adaptation Networks (2015)](http://proceedings.mlr.press/v37/long15.pdf)
* [Deep visual domain adaptation: A survey, 2018](https://arxiv.org/pdf/1802.03601.pdf)
* [A Survey on Deep Transfer Learning, 2018](https://arxiv.org/pdf/1808.01974.pdf)
* [Adversarial Discriminative Domain Adaptation (2017)](http://openaccess.thecvf.com/content_cvpr_2017/papers/Tzeng_Adversarial_Discriminative_Domain_CVPR_2017_paper.pdf)
* [Learning Texture Invariant Representationfor Domain Adaptation of Semantic Segmentation (CVPR 2020)](http://openaccess.thecvf.com/content_CVPR_2020/papers/Kim_Learning_Texture_Invariant_Representation_for_Domain_Adaptation_of_Semantic_Segmentation_CVPR_2020_paper.pdf)  
  * [Pytorch implementation](https://github.com/JitengMu/Learning-from-Synthetic-Animals)
* [IMAGENET-TRAINED CNNS ARE BIASED TOWARDS
TEXTURE; INCREASING SHAPE BIAS IMPROVES
ACCURACY AND ROBUSTNESS](https://arxiv.org/pdf/1811.12231.pdf)

## Tutorials, blogs and more
* [A collection of AWESOME things about domain adaptation (Github)](https://github.com/zhaoxin94/awesome-domain-adaptation#theory)
* [Youtube tutorial on DA (classic and theoretical)](https://www.youtube.com/watch?v=F2OJ0fAK46Q&t=3758s)

## Code
* [Dassl - A PyTorch toolbox for domain adaptation and semi-supervised learning.
](https://github.com/KaiyangZhou/Dassl.pytorch)
