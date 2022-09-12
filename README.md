## Awesome resources on Hyperspectral Image Unmixing
A list of hyperspectral image unmixing resources collected by Xiuheng Wang (xiuheng.wang@oca.eu) and Min Zhao (minzhao@mail.nwpu.edu.cn). **For more details, please refer to our paper: Integration of Physics-Based and Data-Driven Models for Hyperspectral Image Unmixing.** [[Paper](https://arxiv.org/pdf/2206.05508.pdf)]. If you find any important resources are not included, please feel free to contact us.

    @article{chen2022integration,
      title={Integration of Physics-Based and Data-Driven Models for Hyperspectral Image Unmixing},
      author={Chen, Jie and Zhao, Min and Wang, Xiuheng and Richard, C{\'e}dric and Rahardja, Susanto},
      journal={arXiv preprint arXiv:2206.05508},
      year={2022}
    }

## Contents

- [Physics-based mixture model](#model)
  - [Survey](#survey)
  - [Examples](#examples)
- [Classic unmixing methods](#classic)
- [Integrating of physics-based models in DNN design](#network)
- [Prior information learning with data-driven approaches](#iterative)
- [Integrating loss learnt from data into physics-based inverse problems](#loss)
- [Databases](#data)
- [Toolbox](#toolbox)

<a name="model" />

## Physics-based mixture model

<a name="survey" />

### Survey
1. **Advances in hyperspectral image and signal processing: A comprehensive overview of the state of the art.** GRSM 2017, *P. Ghamisi et al*.
[[Paper](https://ieeexplore.ieee.org/stamp/stamp.jsp?tp=&arnumber=8113122)]
2. **Nonlinear unmixing of hyperspectral images: Models and algorithms.** SPM 2013, *N. Dobigeon et al*.
[[Paper](https://ieeexplore.ieee.org/stamp/stamp.jsp?tp=&arnumber=6678284)] 
3. **A review of nonlinear hyperspectral unmixing methods.** JSTARS 2014, *R. Heylen et al*.
[[Paper](https://ieeexplore.ieee.org/stamp/stamp.jsp?tp=&arnumber=6816071)] 
4. **Spectral variability in hyperspectral data unmixing: A comprehensive review.** GRSM 2021, *R. Borsoi et al*.
[[Paper](https://ieeexplore.ieee.org/stamp/stamp.jsp?tp=&arnumber=9439249)] [[Code](https://github.com/ricardoborsoi/unmixing_spectral_variability)] :fire:


<a name="examples" />

### Examples
1. **Nonlinear unmixing of hyperspectral images using a generalized bilinear model.** TGRS 2011, *A. Halimi et al*.
[[Paper](https://ieeexplore.ieee.org/stamp/stamp.jsp?tp=&arnumber=5702384)]
2. **Theory of reflectance and emittance spectroscopy.** Cambridge university press 2012, *B. Hapke*. 
[[Paper](https://www.cambridge.org/core/books/theory-of-reflectance-and-emittance-spectroscopy/C266E1164D5E14DA18141F03D0E0EAB0)]


<a name="classic" />

## Classic unmixing methods
1. **Fully Constrained Least Squares Linear Spectral Mixture Analysis Method for Material Quantification in Hyperspectral Imagery.** TGRS 2001, *D. C. Heinz et al*. [[Paper](https://ieeexplore.ieee.org/stamp/stamp.jsp?tp=&arnumber=911111)]
2. **Endmember extraction from highly mixed data using minimum volume constrained nonnegative matrix factorization.** TGRS 2007, *L Miao et al*.
[[Paper](https://ieeexplore.ieee.org/stamp/stamp.jsp?tp=&arnumber=4106058)]
3. **Low-rank and sparse representation for hyperspectral image processing: A review.** GRSM 2021, *J Peng et al*.
[[Paper](https://ieeexplore.ieee.org/stamp/stamp.jsp?tp=&arnumber=9451654)]
4. **Nonlinear estimation of material abundances in hyperspectral images with ℓ1-norm spatial regularization.** TGRS 2013, *J. Chen et al*.
[[Paper](https://ieeexplore.ieee.org/stamp/stamp.jsp?arnumber=6531654)] [[Code](http://www.jie-chen.com/index.php?nfssp=Reproducible)] :fire:
5. **Kernel-based nonlinear spectral unmixing with dictionary pruning.** RS 2019, *Z. Li et al*.
[[Paper](https://www.mdpi.com/2072-4292/11/5/529/pdf?version=1551778872)]  :fire:
6. **Non-linear spectral unmixing by geodesic simplex volume maximization.** JSTSP 2010, *R. Heylen et al*.
[[Paper](https://ieeexplore.ieee.org/stamp/stamp.jsp?tp=&arnumber=5605217)]
7. **Fully constrained least squares spectral unmixing by simplex projection.** TGRS 2011, *R. Heylen et al*.
[[Paper](https://ieeexplore.ieee.org/stamp/stamp.jsp?tp=&arnumber=5887410)] [[Code](https://sites.google.com/site/robheylenresearch/code/simplex_project.m?attredirects=0&d=1)]
8. **A distance geometric framework for nonlinear hyperspectral unmixing.** JSTARS 2014, *R. Heylen et al*.
[[Paper](https://ieeexplore.ieee.org/stamp/stamp.jsp?tp=&arnumber=6814294)] [[Code](https://sites.google.com/site/robheylenresearch/code/simplex_project_dist.m?attredirects=0&d=1)]

<a name="network" />

## Integrating of physics-based models in DNN design.
1. **EndNet: Sparse autoencoder network for endmember extraction and hyperspectral unmixing.** TGRS 2018, *S. Ozkan et al*.
[[Paper](https://ieeexplore.ieee.org/stamp/stamp.jsp?arnumber=8429926)] [[Code](https://github.com/savasozkan/endnet)]
2. **uDAS: An untied denoising autoencoder with sparsity for spectral unmixing.** TGRS 2018, *Y. Qu et al*.
[[Paper](https://ieeexplore.ieee.org/stamp/stamp.jsp?arnumber=8476591)] [[Code](https://github.com/aicip/uDAS)]
3. **DAEN: Deep autoencoder networks for hyperspectral unmixing.** TGRS 2019, *Y. Su et al*.
[[Paper](https://ieeexplore.ieee.org/stamp/stamp.jsp?tp=&arnumber=8628241)] 
4. **Hyperspectral unmixing using a neural network autoencoder.** IEEE Access 2018, *B. Palsson et al*.
[[Paper](https://ieeexplore.ieee.org/stamp/stamp.jsp?tp=&arnumber=8322133)] [[Code](https://github.com/burknipalsson/hu_autoencoders/blob/main/Method_DAEU.ipynb)]
5. **Convolutional autoencoder for spectral–spatial hyperspectral unmixing.** TGRS 2020, *B. Palsson et al*.
[[Paper](https://ieeexplore.ieee.org/stamp/stamp.jsp?tp=&arnumber=8900297)] [[Code](https://github.com/burknipalsson/hu_autoencoders/blob/main/Method_CNNAEU.ipynb)]
6. **Hyperspectral unmixing using deep convolutional autoencoders in a supervised scenario.** JSTARS 2020, *F. Khajehrayeni et al*.
[[Paper](https://ieeexplore.ieee.org/stamp/stamp.jsp?arnumber=8984691)] 
7. **Nonlinear unmixing of hyperspectral data via deep autoencoder network.** GRSL 2019, *M. Wang et al*.
[[Paper](https://ieeexplore.ieee.org/stamp/stamp.jsp?tp=&arnumber=8667664)] [[Code](https://github.com/zhaomin0101/NAE)] :fire:
8. **LSTM-DNN based autoencoder network for nonlinear hyperspectral image unmixing.** JSTSP 2021, *M. Zhao et al*.
[[Paper](https://ieeexplore.ieee.org/stamp/stamp.jsp?tp=&arnumber=9326377)] :fire:
9. **Hyperspectral unmixing for additive nonlinear models with a 3-D-CNN autoencoder network.** TGRS 2022, *M. Zhao et al*.
[[Paper](https://ieeexplore.ieee.org/stamp/stamp.jsp?tp=&arnumber=9503107)] [[Code](https://github.com/zhaomin0101/3DCNN-var)] :fire:
10. **Deep autoencoders with multitask learning for bilinear hyperspectral unmixing.** TGRS 2020, *Y. Su et al*.
[[Paper](https://ieeexplore.ieee.org/stamp/stamp.jsp?tp=&arnumber=9290391)] 
11. **Unsupervised hyperspectral unmixing via nonlinear autoencoders.** TGRS 2021, *K. T. Shahid et al*.
[[Paper](https://ieeexplore.ieee.org/stamp/stamp.jsp?tp=&arnumber=9432042)] [[Code](https://github.com/KaziTShahid/Nonlinear-Hyperspectral-Unmixing-Autoencoder)]
12. **TANet: An unsupervised two-stream autoencoder network for hyperspectral unmixing.** TGRS 2021, *Q. Jin et al*.
[[Paper](https://ieeexplore.ieee.org/stamp/stamp.jsp?tp=&arnumber=9489359)] [[Code](https://github.com/meixiaoguang/TANet)]
13. **Probabilistic generative model for hyperspectral unmixing accounting for endmember variability.**  TGRS 2022, *S. Shi et al*.
[[Paper](https://ieeexplore.ieee.org/stamp/stamp.jsp?tp=&arnumber=9583297)] [[Code](https://github.com/shuaikaishi/PGMSU)] :fire:
14. **Deep generative endmember modeling: An application to unsupervised spectral unmixing.** TCI 2019, *R. Borsoi et al*.
[[Paper](https://ieeexplore.ieee.org/stamp/stamp.jsp?tp=&arnumber=8878112)] [[Code](https://github.com/ricardoborsoi/Unmixing_with_Deep_Generative_Models)]
15. **Deep half-siamese networks for hyperspectral unmixing.** GRSL 2020, *Z. Han et al*.
[[Paper](https://ieeexplore.ieee.org/stamp/stamp.jsp?tp=&arnumber=9160879)] 
16. **Dual branch autoencoder network for spectral-spatial hyperspectral unmixing.** GRSL 2021, *Z. Hua et al*.
[[Paper](https://ieeexplore.ieee.org/stamp/stamp.jsp?arnumber=9474909)] 
17. **Cycu-net: Cycle-consistency unmixing network by learning cascaded autoencoders.** TGRS 2021, *L. Gao et al*.
[[Paper](https://ieeexplore.ieee.org/stamp/stamp.jsp?tp=&arnumber=9383423)] [[Code](https://github.com/hanzhu97702/IEEE_TGRS_CyCU-Net)]
18. **UnDIP: Hyperspectral unmixing using deep image prior.** TGRS 2021, *B. Rasti et al*. 
[[Paper](https://ieeexplore.ieee.org/stamp/stamp.jsp?tp=&arnumber=9392110)] [[Code](https://github.com/BehnoodRasti/UnDIP)]
19. **SSCU-Net: Spatial–spectral collaborative unmixing network for hyperspectral images.** TGRS 2022, *L. Qi et al*. 
[[Paper](https://ieeexplore.ieee.org/stamp/stamp.jsp?tp=&arnumber=9709843)]
20. **Multimodal hyperspectral unmixing: Insights from attention networks.** TGRS 2022, *Z. Han et al*. 
[[Paper](https://ieeexplore.ieee.org/stamp/stamp.jsp?tp=&arnumber=9724217)] [[Code](https://github.com/hanzhu97702/IEEE_TGRS_MUNet)]

<a name="iterative" />

## Prior information learning with data-driven approaches
1. **A plug-and-play priors framework for hyperspectral unmixing.** TGRS 2021, *M. Zhao et al*.
[[Paper](https://ieeexplore.ieee.org/stamp/stamp.jsp?tp=&arnumber=9325040)] [[Code](https://github.com/xiuheng-wang/Plug_and_Play_HSI_unmixing)] :fire:
2. **Hyperspectral unmixing via nonnegative matrix factorization with handcrafted and learned priors.** GRSL 2021, *M. Zhao et al*.
[[Paper](https://ieeexplore.ieee.org/stamp/stamp.jsp?tp=&arnumber=9321154)] :fire:
3. **Hyperspectral nonlinear unmixing by using plug-and-play prior for abundance maps** RS 2020, *Z. Wang et al*.
[[Paper](https://www.mdpi.com/2072-4292/12/24/4117)] 
4. **An ADMM based network for hyperspectral unmixing tasks.** ICASSP 2021, *C. Zhou et al*.
[[Paper](https://ieeexplore.ieee.org/stamp/stamp.jsp?tp=&arnumber=9414555)] 
5. **SNMF-Net: Learning a deep alternating neural network for hyperspectral unmixing.** TGRS 2021, *F. Xiong et al*.
[[Paper](https://ieeexplore.ieee.org/stamp/stamp.jsp?tp=&arnumber=9444347)] [[Code](http://www.xiongfuli.com/cv/code/SNMF.zip)]


<a name="loss" />

## Integrating loss learnt from data into physics-based inverse problems
1. **JMnet: Joint metric neural network for hyperspectral unmixing.** TGRS 2021, *A. Min et al*.
[[Paper](https://ieeexplore.ieee.org/stamp/stamp.jsp?tp=&arnumber=9404359)] 
2. **Adversarial autoencoder network for hyperspectral unmixing.** TNNLS 2021, *Q. Jin et al*.
[[Paper](https://ieeexplore.ieee.org/stamp/stamp.jsp?tp=&arnumber=9565143)] [[Code](https://github.com/meixiaoguang/AAENet)]

<a name="data" />

## Databases

1. **A laboratory-created dataset with ground truth for hyperspectral unmixing evaluation.** JSTARS 2019, *M. Zhao et al*.
[[Paper](https://ieeexplore.ieee.org/stamp/stamp.jsp?tp=&arnumber=8681610)] [[Data](http://www.jie-chen.com/index.php?nfssp=Data)] :fire:

<a name="toolbox" />

## Toolbox

1. **Blind hyperspectral unmixing using autoencoders: A critical comparison.** JSTARS 2022, *B. Palsson et al*.
[[Paper](https://ieeexplore.ieee.org/stamp/stamp.jsp?arnumber=9672688)] [[Code](https://github.com/burknipalsson/hu_autoencoders)]
