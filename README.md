# XAI Project 5

This repository contains the dataset preparation and CLIP embedding extraction notebooks for the Project 5 pipeline.

The data is prepared from the Kaggle MIMIC-CXR dataset. The selected images are AP/PA frontal chest X-rays, and the extracted embeddings are intended to be used for the concept discovery part of the project.

## Notebooks

- `kaggle_subset_creation.ipynb`: prepares the image subsets from the Kaggle dataset.
- `colab_clip_embeddings.ipynb`: extracts CLIP embeddings from the prepared subsets in Google Colab.

## Dataset

Dataset used:

- Kaggle `mimic-cxr-dataset`

Image selection:

- AP/PA frontal chest X-rays only

## Prepared Data

Two image subsets were prepared:

| Subset | Purpose |
|---|---|
| 500 images | Small test subset |
| 3000 images | Main subset |

## CLIP Embeddings

Embeddings were extracted using:

| Item | Value |
|---|---|
| Model | CLIP ViT-B/32 |
| Pretraining | OpenAI |
| Embedding size | 512 |

Generated embedding files:

| File | Shape |
|---|---|
| `image_embeddings_500_clip.npy` | `(500, 512)` |
| `image_embeddings_3000_clip.npy` | `(3000, 512)` |

Each embedding has a matching row in the metadata file.

Metadata files:

- `metadata_with_embeddings_500.csv`
- `metadata_with_embeddings_3000.csv`

The metadata includes the image id, image path, view, and subject id.
The metadata files are included inside the embedding output zip files.

## Drive Links

Prepared image subsets:

- 500-image subset: [LINK](https://drive.google.com/file/d/1KpdQVSqh930ZSjO8FzLORWlyPC4xWdd5/view?usp=drive_link)
- 3000-image subset: [LINK](https://drive.google.com/file/d/15oOxS06Cl3iYQXfW1NipXJnzH824-Xbf/view?usp=drive_link)

CLIP embedding outputs:

- 500-image embeddings: [LINK](https://drive.google.com/file/d/1FkHQslaldghFBxGT4gS38n-Doo31BHey/view?usp=drive_link)
- 3000-image embeddings: [LINK](https://drive.google.com/file/d/1XiAFktfHZxHEbv9ET_3ohAVKRUkA2uM3/view?usp=drive_link)