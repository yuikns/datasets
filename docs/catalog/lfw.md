<div itemscope itemtype="http://schema.org/Dataset">
  <div itemscope itemprop="includedInDataCatalog" itemtype="http://schema.org/DataCatalog">
    <meta itemprop="name" content="TensorFlow Datasets" />
  </div>

  <meta itemprop="name" content="lfw" />
  <meta itemprop="description" content="Labeled Faces in the Wild:&#10;        A Database for Studying Face Recognition in&#10;        Unconstrained Environments&#10;&#10;To use this dataset:&#10;&#10;```python&#10;import tensorflow_datasets as tfds&#10;&#10;ds = tfds.load('lfw', split='train')&#10;for ex in ds.take(4):&#10;  print(ex)&#10;```&#10;&#10;See [the guide](https://www.tensorflow.org/datasets/overview) for more&#10;informations on [tensorflow_datasets](https://www.tensorflow.org/datasets).&#10;&#10;" />
  <meta itemprop="url" content="https://www.tensorflow.org/datasets/catalog/lfw" />
  <meta itemprop="sameAs" content="http://vis-www.cs.umass.edu/lfw" />
  <meta itemprop="citation" content="@TechReport{LFWTech,&#10;    author = {Gary B. Huang and Manu Ramesh and Tamara Berg and Erik Learned-Miller},&#10;    title = {Labeled Faces in the Wild: A Database for Studying Face Recognition in Unconstrained Environments},&#10;    institution = {University of Massachusetts, Amherst},&#10;    year = 2007,&#10;    number = {07-49},&#10;    month = {October}&#10;}&#10;" />
</div>

# `lfw`

Labeled Faces in the Wild: A Database for Studying Face Recognition in
Unconstrained Environments

*   URL: [http://vis-www.cs.umass.edu/lfw](http://vis-www.cs.umass.edu/lfw)
*   `DatasetBuilder`:
    [`tfds.image.lfw.LFW`](https://github.com/tensorflow/datasets/tree/master/tensorflow_datasets/image/lfw.py)
*   Version: `v0.1.0`
*   Versions:

    *   **`0.1.0`** (default):

*   Size: `172.20 MiB`

## Features
```python
FeaturesDict({
    'image': Image(shape=(250, 250, 3), dtype=tf.uint8),
    'label': Text(shape=(), dtype=tf.string),
})
```

## Statistics

Split | Examples
:---- | -------:
ALL   | 13,233
TRAIN | 13,233

## Urls

*   [http://vis-www.cs.umass.edu/lfw](http://vis-www.cs.umass.edu/lfw)

## Supervised keys (for `as_supervised=True`)
`(u'label', u'image')`

## Citation
```
@TechReport{LFWTech,
    author = {Gary B. Huang and Manu Ramesh and Tamara Berg and Erik Learned-Miller},
    title = {Labeled Faces in the Wild: A Database for Studying Face Recognition in Unconstrained Environments},
    institution = {University of Massachusetts, Amherst},
    year = 2007,
    number = {07-49},
    month = {October}
}
```

--------------------------------------------------------------------------------
