<div itemscope itemtype="http://schema.org/Dataset">
  <div itemscope itemprop="includedInDataCatalog" itemtype="http://schema.org/DataCatalog">
    <meta itemprop="name" content="TensorFlow Datasets" />
  </div>

  <meta itemprop="name" content="clevr" />
  <meta itemprop="description" content="CLEVR is a diagnostic dataset that tests a range of visual reasoning abilities.&#10;It contains minimal biases and has detailed annotations describing the kind of&#10;reasoning each question requires.&#10;&#10;&#10;To use this dataset:&#10;&#10;```python&#10;import tensorflow_datasets as tfds&#10;&#10;ds = tfds.load('clevr', split='train')&#10;for ex in ds.take(4):&#10;  print(ex)&#10;```&#10;&#10;See [the guide](https://www.tensorflow.org/datasets/overview) for more&#10;informations on [tensorflow_datasets](https://www.tensorflow.org/datasets).&#10;&#10;" />
  <meta itemprop="url" content="https://www.tensorflow.org/datasets/catalog/clevr" />
  <meta itemprop="sameAs" content="https://cs.stanford.edu/people/jcjohns/clevr/" />
  <meta itemprop="citation" content="@inproceedings{johnson2017clevr,&#10;  title={{CLEVR}: A diagnostic dataset for compositional language and elementary visual reasoning},&#10;  author={Johnson, Justin and Hariharan, Bharath and van der Maaten, Laurens and Fei-Fei, Li and Lawrence Zitnick, C and Girshick, Ross},&#10;  booktitle={Proceedings of the IEEE Conference on Computer Vision and Pattern Recognition},&#10;  year={2017}&#10;}&#10;" />
</div>

# `clevr`

CLEVR is a diagnostic dataset that tests a range of visual reasoning abilities.
It contains minimal biases and has detailed annotations describing the kind of
reasoning each question requires.

*   URL:
    [https://cs.stanford.edu/people/jcjohns/clevr/](https://cs.stanford.edu/people/jcjohns/clevr/)
*   `DatasetBuilder`:
    [`tfds.image.clevr.CLEVR`](https://github.com/tensorflow/datasets/tree/master/tensorflow_datasets/image/clevr.py)
*   Version: `v1.0.0`
*   Versions:

    *   **`1.0.0`** (default):
    *   `3.0.0`: New split API (https://tensorflow.org/datasets/splits)

*   Size: `17.72 GiB`

## Features
```python
FeaturesDict({
    'file_name': Text(shape=(), dtype=tf.string),
    'image': Image(shape=(None, None, 3), dtype=tf.uint8),
    'objects': Sequence({
        '3d_coords': Tensor(shape=(3,), dtype=tf.float32),
        'color': ClassLabel(shape=(), dtype=tf.int64, num_classes=8),
        'material': ClassLabel(shape=(), dtype=tf.int64, num_classes=2),
        'pixel_coords': Tensor(shape=(3,), dtype=tf.float32),
        'rotation': Tensor(shape=(), dtype=tf.float32),
        'shape': ClassLabel(shape=(), dtype=tf.int64, num_classes=3),
        'size': ClassLabel(shape=(), dtype=tf.int64, num_classes=2),
    }),
})
```

## Statistics

Split      | Examples
:--------- | -------:
ALL        | 100,000
TRAIN      | 70,000
TEST       | 15,000
VALIDATION | 15,000

## Urls

*   [https://cs.stanford.edu/people/jcjohns/clevr/](https://cs.stanford.edu/people/jcjohns/clevr/)

## Citation
```
@inproceedings{johnson2017clevr,
  title={{CLEVR}: A diagnostic dataset for compositional language and elementary visual reasoning},
  author={Johnson, Justin and Hariharan, Bharath and van der Maaten, Laurens and Fei-Fei, Li and Lawrence Zitnick, C and Girshick, Ross},
  booktitle={Proceedings of the IEEE Conference on Computer Vision and Pattern Recognition},
  year={2017}
}
```

--------------------------------------------------------------------------------
