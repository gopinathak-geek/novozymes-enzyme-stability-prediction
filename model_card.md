# Model Card

The model analyzed in this card predicts the melting point of the enzyme.

On this page, you can learn more about how well the model performs on the given protein sequence.

## Model Description

**Input:** Protein sequence and Ph

**Output:** Melting temperature of the enzyme

**Model Architecture:** Novonet - Convolution neural network

## Performance

The performance of the model was evaluated on the [Spearman's correlation coefficient](https://en.wikipedia.org/wiki/Spearman%27s_rank_correlation_coefficient) between the ground truth and the predictions.

This model does not perform well, since this model consider only the molecular weight of the amino acid and the ph. To improve this model performace we need to get the other important features of the amino acids

## Limitations

Presently the model cannot be used for the predection, we need to improve the performace of the model.

## Trade-offs

The model cannot be user for the predection but by this model we studied that the melting temperature of the protein does not rely only upon the molecular weight of the amino acid.
