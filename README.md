# Domain-Adaptation

## Papers
* [Ship classification from overhead imageryusing synthetic data and domain adaptation (2019)](https://arxiv.org/pdf/1905.03894.pdf)
  * Building a large (200k) dataset of sythetic ships and using it to increase classification performance with domain adaptation
* [Unsupervised Domain Adaptation by Backpropagation (2015)](https://arxiv.org/pdf/1409.7495.pdf)  
  * Train a NN to discriminate between different classes while being invariant with respect to the shift between the domains.
  * Simple and easy to implement.
* [Unsupervised Pixel-Level Domain Adaptation With Generative Adversarial Networks (2017)](http://openaccess.thecvf.com/content_cvpr_2017/html/Bousmalis_Unsupervised_Pixel-Level_Domain_CVPR_2017_paper.html)  
  * [CVPR 2017 oral](https://www.youtube.com/watch?v=VhsTrWPvjcA)
* [Maximum Classifier Discrepancy for Unsupervised Domain Adaptation](http://openaccess.thecvf.com/content_cvpr_2018/papers/Saito_Maximum_Classifier_Discrepancy_CVPR_2018_paper.pdf)  
  * Train two different classifiers for the source while maximizing the discrepancy between them. Meanwhile, train the feature generator to minimize the discrepancy. 
  * [Code](https://github.com/mil-tokyo/MCD_DA/tree/master/classification)
   * [CVPR 2018 oral](https://www.youtube.com/watch?v=8mk7i3vGjAM)
* [Deep visual domain adaptation: A survey, 2018](https://arxiv.org/pdf/1802.03601.pdf)
* [A Survey on Deep Transfer Learning, 2018](https://arxiv.org/pdf/1808.01974.pdf)
* [Adversarial Discriminative Domain Adaptation (2017)](http://openaccess.thecvf.com/content_cvpr_2017/papers/Tzeng_Adversarial_Discriminative_Domain_CVPR_2017_paper.pdf)
* [Deep CORAL: Correlation Alignment for Deep Domain Adaptation (2016)](https://arxiv.org/pdf/1607.01719.pdf)
* [Learning from Synthetic Animals (CVPR 2020)](https://arxiv.org/pdf/1912.08265.pdf)
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
