# Domain-Adaptation

## Papers
### Adverserial Methods:
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
* [Learning from Synthetic Data: Addressing Domain Shift for SemanticSegmentation (2018)](https://openaccess.thecvf.com/content_cvpr_2018/papers/Sankaranarayanan_Learning_From_Synthetic_CVPR_2018_paper.pdf)
  * A 4 blocks architecture trained separately for bridging the gap between real and fake images (semantic segmentation)   
* [Unsupervised Domain Adaptation with Similarity Learning (CVPR 2018)](https://openaccess.thecvf.com/content_cvpr_2018/papers/Pinheiro_Unsupervised_Domain_Adaptation_CVPR_2018_paper.pdf)  
  * Train two different networkes: 1. Generate features that are domain invariant (and also good for the similarity operation mensioned below). 2. Generate features that the similarity between them and the first features indicates the classes. 
  * What is the advantage of this method compared to the calssic advarsial approach?  
 * [Adversarial Discriminative Domain Adaptation (2017)](http://openaccess.thecvf.com/content_cvpr_2017/papers/Tzeng_Adversarial_Discriminative_Domain_CVPR_2017_paper.pdf)
* [Discriminative Adversarial Domain Adaptation (AAAI 2020)](https://arxiv.org/pdf/1911.12036v2.pdf)
  * State-of-the-art on Syn2Real - [79.8%](https://paperswithcode.com/sota/synthetic-to-real-translation-on-syn2real-c)(but it is a new dataset, so other methods may be better but didn't try).
### Distance Based Methods
* [Deep CORAL: Correlation Alignment for Deep Domain Adaptation (2016)](https://arxiv.org/pdf/1607.01719.pdf)
  * Minimize a CORAL loss, i.e. minimize the difference between the second moment of the source feautres and the second moment of the target features.
* [d-SNE: Domain Adaptation using Stochastic Neighborhood Embedding (CVPR 2019](https://openaccess.thecvf.com/content_CVPR_2019/papers/Xu_d-SNE_Domain_Adaptation_Using_Stochastic_Neighborhood_Embedding_CVPR_2019_paper.pdf)
  * Assumes that we have few lables of the target domain (not alwayes true!).
  * Traines two neural networks to generate features from the source and target such that features of insntances from the same classes will be close.
  * Good resuls on visDA2017: [86.15%](https://paperswithcode.com/sota/domain-adaptation-on-visda2017). 
### Discrepancy Based Methods:
* [Contrastive Adaptation Network for Unsupervised Domain Adaptation (CVPR 2019)](https://openaccess.thecvf.com/content_CVPR_2019/papers/Kang_Contrastive_Adaptation_Network_for_Unsupervised_Domain_Adaptation_CVPR_2019_paper.pdf)
  * State-of-the-art results on office-31 dataset [(90.6%](https://paperswithcode.com/sota/domain-adaptation-on-office-31)) and visDA2017 ([87.2%](https://paperswithcode.com/sota/domain-adaptation-on-visda2017)).
* [Learning Transferable Features with Deep Adaptation Networks (2015)](http://proceedings.mlr.press/v37/long15.pdf)
### Others Methods:
* [Fully Test-time Adaptation by Entropy Minimization (2020)](https://arxiv.org/pdf/2006.10726.pdf)
  * Apply a few iteration of minimizing the entropy of the NN on the target samples. 
  * Relatively easy to implement and fast.
* [Learning from Synthetic Animals (CVPR 2020)](https://arxiv.org/pdf/1912.08265.pdf)
  * Generate Pseudo-Labels by iteratively apply the current model and check the consistencies of it.
  * Augment the synthetic data - "An animal with random poses and random texture is rendered from a random viewpoint for some random lighting
and a random background image."
* [Learning Texture Invariant Representationfor Domain Adaptation of Semantic Segmentation (CVPR 2020)](http://openaccess.thecvf.com/content_CVPR_2020/papers/Kim_Learning_Texture_Invariant_Representation_for_Domain_Adaptation_of_Semantic_Segmentation_CVPR_2020_paper.pdf)  
  * [Pytorch implementation](https://github.com/JitengMu/Learning-from-Synthetic-Animals)
* [Ship classification from overhead imagery using synthetic data and domain adaptation (2019)](https://arxiv.org/pdf/1905.03894.pdf)
  * Building a large (200k) dataset of synthetic ships and using it to increase classification performance with domain adaptation
  * Looks like they just added images to training set, and not a special domain adaptation
* [IMAGENET-TRAINED CNNS ARE BIASED TOWARDS
TEXTURE; INCREASING SHAPE BIAS IMPROVES
ACCURACY AND ROBUSTNESS](https://arxiv.org/pdf/1811.12231.pdf)
### Surveys
* [Deep visual domain adaptation: A survey, 2018](https://arxiv.org/pdf/1802.03601.pdf)
* [A Survey on Deep Transfer Learning, 2018](https://arxiv.org/pdf/1808.01974.pdf)


## Datasets
* [Syn2Real](http://ai.bu.edu/syn2real/) - A New Benchmark for
Synthetic-to-Real Visual Domain Adaptation.
* Ofice31.
## Tutorials, blogs and more
* [A collection of AWESOME things about domain adaptation (Github)](https://github.com/zhaoxin94/awesome-domain-adaptation#theory)
* [Youtube tutorial on DA (classic and theoretical)](https://www.youtube.com/watch?v=F2OJ0fAK46Q&t=3758s)

## Code
* [Dassl - A PyTorch toolbox for domain adaptation and semi-supervised learning.
](https://github.com/KaiyangZhou/Dassl.pytorch)
