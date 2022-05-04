The process of generating synthetic data for ML use cases is an open technical challenge. Here we list a lightly annotated bibliography of reference sources on how to generate datasets to test for bias:

Imperfect ImaGINation: Implications of GANs Exacerbating Biases on Facial Data (2021) -- GANs, a popular technique for data generation, were shown to introduce bias into real-world datasets. Recommendations on methods to use to limit bias.

Bayesian Perspective on Visual Data Augmentation for Efficient Utilization of Sub-sampled Data (2021) -- The authors introduce methods for sub-sampling pools of data that better represent data distribution based on estimated uncertainty measures they introduce. Data generation comes into play in the crucial blanks of the sub-sampled data pool to represent the overall distribution, which can then be used for more effective training of ML models such that bias is reduced.

Synthetic data for model selection (Fitz et al., 2021). Synthetic generation pipelines are useful in that they generate an unlimited number of objects (text snippets, images). The authors propose funneling these objects, in the context of highly photorealistic images, into machine learning (ML) pipelines. The notable point of this paper is that, while research in this field has focused on using synthetic images for training, by augmenting and enlarging training data the authors explore whether synthetic data can be beneficial for model selection. Considering the task of image classification, we demonstrate that when data is scarce, synthetic data can be used to replace the held out validation set, thus allowing modelers to train on a larger dataset.

FFPDG: Fast, Fair and Private Data Generation (Amazon Research, 2021 Workshop 2022 Conference). The authors explicitly take into account the effects of fairness and computational resources while generating data for training and validation purposes. Note that they also show how to impose a privacy constraint.

https://github.com/BorealisAI/private-data-generation, 2019 -- private data generation repository

Fair-max-entropy-distributions https://github.com/vijaykeswani, 2020 -- fair maximum entropy distribution that describes a set of metrics against which sampled/synthetic data is measured to ensure maximum of the distributional span within fairness constraints.

Optimized data pre-processing for discrimination prevention. This paper provides methods that can be adapted to synthetic data generation for smoothing out biases and overweights on certain elements of the distribution. While not explicitly applied to synthetic data generation in the paper, the methods are transferable between tasks.
