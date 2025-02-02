<div itemscope itemtype="http://schema.org/Dataset">
  <div itemscope itemprop="includedInDataCatalog" itemtype="http://schema.org/DataCatalog">
    <meta itemprop="name" content="TensorFlow Datasets" />
  </div>

  <meta itemprop="name" content="patch_camelyon" />
  <meta itemprop="description" content="The PatchCamelyon benchmark is a new and challenging image classification&#10;dataset. It consists of 327.680 color images (96 x 96px) extracted from&#10;histopathologic scans of lymph node sections. Each image is annoted with a&#10;binary label indicating presence of metastatic tissue. PCam provides a new&#10;benchmark for machine learning models: bigger than CIFAR10, smaller than&#10;Imagenet, trainable on a single GPU.&#10;&#10;&#10;To use this dataset:&#10;&#10;```python&#10;import tensorflow_datasets as tfds&#10;&#10;ds = tfds.load('patch_camelyon', split='train')&#10;for ex in ds.take(4):&#10;  print(ex)&#10;```&#10;&#10;See [the guide](https://www.tensorflow.org/datasets/overview) for more&#10;informations on [tensorflow_datasets](https://www.tensorflow.org/datasets).&#10;&#10;" />
  <meta itemprop="url" content="https://www.tensorflow.org/datasets/catalog/patch_camelyon" />
  <meta itemprop="sameAs" content="https://patchcamelyon.grand-challenge.org/" />
  <meta itemprop="citation" content="@misc{b_s_veeling_j_linmans_j_winkens_t_cohen_2018_2546921,&#10;  author       = {B. S. Veeling, J. Linmans, J. Winkens, T. Cohen, M. Welling},&#10;  title        = {Rotation Equivariant CNNs for Digital Pathology},&#10;  month        = sep,&#10;  year         = 2018,&#10;  doi          = {10.1007/978-3-030-00934-2_24},&#10;  url          = {https://doi.org/10.1007/978-3-030-00934-2_24}&#10;}&#10;" />
</div>

# `patch_camelyon`

The PatchCamelyon benchmark is a new and challenging image classification
dataset. It consists of 327.680 color images (96 x 96px) extracted from
histopathologic scans of lymph node sections. Each image is annoted with a
binary label indicating presence of metastatic tissue. PCam provides a new
benchmark for machine learning models: bigger than CIFAR10, smaller than
Imagenet, trainable on a single GPU.

*   URL:
    [https://patchcamelyon.grand-challenge.org/](https://patchcamelyon.grand-challenge.org/)
*   `DatasetBuilder`:
    [`tfds.image.patch_camelyon.PatchCamelyon`](https://github.com/tensorflow/datasets/tree/master/tensorflow_datasets/image/patch_camelyon.py)
*   Version: `v0.1.0`
*   Versions:

    *   **`0.1.0`** (default):
    *   `2.0.0`: New split API (https://tensorflow.org/datasets/splits)

*   Size: `7.48 GiB`

## Features
```python
FeaturesDict({
    'id': Text(shape=(), dtype=tf.string),
    'image': Image(shape=(96, 96, 3), dtype=tf.uint8),
    'label': ClassLabel(shape=(), dtype=tf.int64, num_classes=2),
})
```

## Statistics

Split      | Examples
:--------- | -------:
ALL        | 327,680
TRAIN      | 262,144
TEST       | 32,768
VALIDATION | 32,768

## Urls

*   [https://patchcamelyon.grand-challenge.org/](https://patchcamelyon.grand-challenge.org/)

## Supervised keys (for `as_supervised=True`)
`(u'image', u'label')`

## Citation
```
@misc{b_s_veeling_j_linmans_j_winkens_t_cohen_2018_2546921,
  author       = {B. S. Veeling, J. Linmans, J. Winkens, T. Cohen, M. Welling},
  title        = {Rotation Equivariant CNNs for Digital Pathology},
  month        = sep,
  year         = 2018,
  doi          = {10.1007/978-3-030-00934-2_24},
  url          = {https://doi.org/10.1007/978-3-030-00934-2_24}
}
```

--------------------------------------------------------------------------------
