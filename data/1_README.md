# Data Files

This folder contains the data and outputs generated throughout the step number 2 of the project.

### Part 2 Outputs

* `sae_model.pt` — Trained Sparse Autoencoder model.
* `sae_activations.npy` — SAE activations computed for all image embeddings.
* `training_loss.csv` — Training loss history of the Sparse Autoencoder.
* `activation_stats.csv` — Statistics used to identify dead, rare, and over-activated neurons.
* `neuron_to_concept.json` — Mapping from SAE neurons to discovered concept names.
* `neuron_to_concept.csv` — Tabular version of the neuron-to-concept mapping.
* `image_concepts_filtered.json` — Final concept explanations generated for each image.
* `image_concepts_filtered.csv` — Tabular version of the image-level concepts.
* `image_concepts_unfiltered.json` — Image concepts before reliability filtering.
* `image_concepts_unfiltered.csv` — Tabular version of the unfiltered image concepts.
* `reliability_report.json` — Summary of all reliability evaluation results.

### Reliability Evaluation Outputs

* `semantic_alignment_summary.csv` — Measures concept naming confidence using cosine similarity scores.
* `before_after_filtering_summary.csv` — Comparison of explanations before and after reliability filtering.
* `generalness_filtered.csv` — Analysis of concept over-activation and generalness.
* `generalness_unfiltered.csv` — Generalness analysis before filtering.
* `similar_image_consistency_pairs.csv` — Pairwise concept consistency between nearest-neighbor images.
* `similar_image_consistency_summary.csv` — Aggregate consistency statistics across similar images.
* `concept_consistency_filtered.csv` — Concept-level consistency scores after filtering.
* `concept_consistency_unfiltered.csv` — Concept-level consistency scores before filtering.


