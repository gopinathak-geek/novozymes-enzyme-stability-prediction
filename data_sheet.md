# Datasheet Template

## Motivation

For the training set, the protein thermostability (experimental melting temperature) data includes natural sequences, as well as engineered sequences with single or multiple mutations upon the natural sequences. The data are mainly from different sources of published studies such as [Meltome atlas—thermal proteome stability across the tree of life](https://www.nature.com/articles/s41592-020-0801-4). Many other public datasets exist for protein stability; please see the competition [Rule 7C](https://www.kaggle.com/competitions/novozymes-enzyme-stability-prediction/rules) for external data usage requirements. There are also other publicly available methods which can predict protein stabilities such as [ESM](https://www.pnas.org/doi/full/10.1073/pnas.2016239118), [EVE](https://www.nature.com/articles/s41586-021-04043-8) and [Rosetta](https://www.sciencedirect.com/science/article/abs/pii/B9780123812704000196?via%3Dihub) etc., without using the provided training set. These methods may also be used as part of the competition.

 
## Composition

- seq_id: unique identifier of each protein variants
- protein_sequence: amino acid sequence of each protein variant. The stability (as measured by tm) of protein is determined by its protein sequence. (Please note that most of the sequences in the test data have the same length of 221 amino acids, but some of them have 220 because of amino acid deletion.)
- pH: the scale used to specify the acidity of an aqueous solution under which the stability of protein was measured. Stability of the same protein can change at different pH levels.
- data_source: source where the data was published
- tm: target column. Since only the spearman correlation will be used for the evaluation, the correct prediction of the relative order is more important than the absolute tm values. (Higher tm means the protein variant is more stable.)

## Collection process

The data is provided by the competetion host

## Preprocessing/cleaning/labelling

The train data contains some improper information, the host has provided the update of the training data, so the training data is modified accoriding to the updated information
 

## Maintenance

[Novoenzymes](https://www.novozymes.com/en)

