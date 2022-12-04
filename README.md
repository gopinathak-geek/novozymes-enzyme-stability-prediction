# Novozymes Enzyme Stability Prediction


## Goal of the Competition
Enzymes are proteins that act as catalysts in the chemical reactions of living organisms. The goal of this competition is to predict the thermostability of enzyme variants. The experimentally measured thermostability (melting temperature) data includes natural sequences, as well as engineered sequences with single or multiple mutations upon the natural sequences.

Understanding and accurately predict protein stability is a fundamental problem in biotechnology. Its applications include enzyme engineering for addressing the world’s challenges in sustainability, carbon neutrality and more. Improvements to enzyme stability could lower costs and increase the speed scientists can iterate on concepts.

## DATA
For the training set, the protein thermostability (experimental melting temperature) data includes natural sequences, as well as engineered sequences with single or multiple mutations upon the natural sequences. The data are mainly from different sources of published studies such as [Meltome atlas—thermal proteome stability across the tree of life](https://www.nature.com/articles/s41592-020-0801-4). Many other public datasets exist for protein stability; please see the competition [Rule 7C](https://www.kaggle.com/competitions/novozymes-enzyme-stability-prediction/rules) for external data usage requirements. There are also other publicly available methods which can predict protein stabilities such as [ESM](https://www.pnas.org/doi/full/10.1073/pnas.2016239118), [EVE](https://www.nature.com/articles/s41586-021-04043-8) and [Rosetta](https://www.sciencedirect.com/science/article/abs/pii/B9780123812704000196?via%3Dihub) etc., without using the provided training set. These methods may also be used as part of the competition.

The test set contains experimental melting temperature of over 2,413 single-mutation variant of an enzyme (GenBank: KOC15878.1), obtained by Novozymes A/S. The amino acid sequence of the wild type is:

VPVNPEPDATSVENVALKTGSGDSQSDPIKADLEVKGQSALPFDVDCWAILCKGAPNVLQRVNEKTKNSNRDRSGANKGPFKDPQKWGIKALPPKNPSWSAQDFKSPEEYAFASSLQGGTNAILAPVNLASQNSQGGVLNGFYSANKVAQFDPSKPQQTKGTWFQITKFTGAAGPYCKALGSNDKSVCDKNKNIAGDWGFDPAKWAYQYDEKNNKFNYVGK

## MODEL 
For this competetion the model used is Convolution neural network. The behaviour of the protein is based on the 3d structure and the folding structure is based on the combination of 20 amino acids. Since the protein folding is depends upon the combination the CNN will find the important feature and predict.

## HYPERPARAMETER OPTIMSATION
[Optuna](https://optuna.org/) - A hyper parameter optimization framework is used to tune the hyper parameter and the following hyperparametes are tuned

* Number of Fully connected layers in the CNN
* Number of units in each layer
* Drop out
* optimizer
* Learning rate

## RESULTS
This model is developed by considering the feature - molecular weight of the amino acid the maximum accuracy for this model is 0.20.
This model did not perform well, so we need to develop the model considering the other factors of the amino acids


## CONTACT DETAILS
* Name - Gopinath Alagar Karunanithi
* LinkedIn - [LinkedIn](https://www.linkedin.com/in/gopinathak/)
* Gmail - <gopinathak.geek@gmail.com>
