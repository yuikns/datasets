<div itemscope itemtype="http://schema.org/Dataset">
  <div itemscope itemprop="includedInDataCatalog" itemtype="http://schema.org/DataCatalog">
    <meta itemprop="name" content="TensorFlow Datasets" />
  </div>

  <meta itemprop="name" content="so2sat" />
  <meta itemprop="description" content="So2Sat LCZ42 is a dataset consisting of co-registered synthetic aperture radar&#10;and multispectral optical image patches acquired by the Sentinel-1 and&#10;Sentinel-2 remote sensing satellites, and the corresponding local climate zones&#10;(LCZ) label. The dataset is distributed over 42 cities across different&#10;continents and cultural regions of the world.&#10;&#10;The full dataset (`all`) consists of 8 Sentinel-1 and 10 Sentinel-2 channels.&#10;Alternatively, one can select the `rgb` subset, which contains only the optical&#10;frequency bands of Sentinel-2, rescaled and encoded as JPEG.&#10;&#10;Dataset URL: http://doi.org/10.14459/2018MP1454690&#10;License: http://creativecommons.org/licenses/by/4.0&#10;&#10;&#10;To use this dataset:&#10;&#10;```python&#10;import tensorflow_datasets as tfds&#10;&#10;ds = tfds.load('so2sat', split='train')&#10;for ex in ds.take(4):&#10;  print(ex)&#10;```&#10;&#10;See [the guide](https://www.tensorflow.org/datasets/overview) for more&#10;informations on [tensorflow_datasets](https://www.tensorflow.org/datasets).&#10;&#10;" />
  <meta itemprop="url" content="https://www.tensorflow.org/datasets/catalog/so2sat" />
  <meta itemprop="sameAs" content="http://doi.org/10.14459/2018MP1454690" />
  <meta itemprop="citation" content="" />
</div>

# `so2sat`

So2Sat LCZ42 is a dataset consisting of co-registered synthetic aperture radar
and multispectral optical image patches acquired by the Sentinel-1 and
Sentinel-2 remote sensing satellites, and the corresponding local climate zones
(LCZ) label. The dataset is distributed over 42 cities across different
continents and cultural regions of the world.

The full dataset (`all`) consists of 8 Sentinel-1 and 10 Sentinel-2 channels.
Alternatively, one can select the `rgb` subset, which contains only the optical
frequency bands of Sentinel-2, rescaled and encoded as JPEG.

Dataset URL: http://doi.org/10.14459/2018MP1454690 License:
http://creativecommons.org/licenses/by/4.0

*   URL:
    [http://doi.org/10.14459/2018MP1454690](http://doi.org/10.14459/2018MP1454690)
*   `DatasetBuilder`:
    [`tfds.image.so2sat.So2sat`](https://github.com/tensorflow/datasets/tree/master/tensorflow_datasets/image/so2sat.py)

`so2sat` is configured with `tfds.image.so2sat.So2satConfig` and has the
following configurations predefined (defaults to the first one):

*   `rgb` (`v0.0.1`) (`Size: ?? GiB`): Sentinel-2 RGB channels

*   `all` (`v0.0.1`) (`Size: ?? GiB`): 8 Sentinel-1 and 10 Sentinel-2 channels

## `so2sat/rgb`
Sentinel-2 RGB channels

Versions:

*   **`0.0.1`** (default):
*   `2.0.0`: New split API (https://tensorflow.org/datasets/splits)

### Statistics
None computed

### Features
```python
FeaturesDict({
    'image': Image(shape=(32, 32, 3), dtype=tf.uint8),
    'label': ClassLabel(shape=(), dtype=tf.int64, num_classes=17),
    'sample_id': Tensor(shape=(), dtype=tf.int64),
})
```

### Urls

*   [http://doi.org/10.14459/2018MP1454690](http://doi.org/10.14459/2018MP1454690)

### Supervised keys (for `as_supervised=True`)
`(u'image', u'label')`

## `so2sat/all`
8 Sentinel-1 and 10 Sentinel-2 channels

Versions:

*   **`0.0.1`** (default):
*   `2.0.0`: New split API (https://tensorflow.org/datasets/splits)

### Statistics
None computed

### Features
```python
FeaturesDict({
    'label': ClassLabel(shape=(), dtype=tf.int64, num_classes=17),
    'sample_id': Tensor(shape=(), dtype=tf.int64),
    'sentinel1': Tensor(shape=[32, 32, 8], dtype=tf.float32),
    'sentinel2': Tensor(shape=[32, 32, 10], dtype=tf.float32),
})
```

### Urls

*   [http://doi.org/10.14459/2018MP1454690](http://doi.org/10.14459/2018MP1454690)

--------------------------------------------------------------------------------
