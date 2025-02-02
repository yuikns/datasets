<div itemscope itemtype="http://schema.org/Dataset">
  <div itemscope itemprop="includedInDataCatalog" itemtype="http://schema.org/DataCatalog">
    <meta itemprop="name" content="TensorFlow Datasets" />
  </div>

  <meta itemprop="name" content="scene_parse150" />
  <meta itemprop="description" content="&#10;Scene parsing is to segment and parse an image into different image regions&#10;associated with semantic categories, such as sky, road, person, and bed.&#10;MIT Scene Parsing Benchmark (SceneParse150) provides a standard training and&#10;evaluation platform for the algorithms of scene parsing.&#10;&#10;&#10;To use this dataset:&#10;&#10;```python&#10;import tensorflow_datasets as tfds&#10;&#10;ds = tfds.load('scene_parse150', split='train')&#10;for ex in ds.take(4):&#10;  print(ex)&#10;```&#10;&#10;See [the guide](https://www.tensorflow.org/datasets/overview) for more&#10;informations on [tensorflow_datasets](https://www.tensorflow.org/datasets).&#10;&#10;" />
  <meta itemprop="url" content="https://www.tensorflow.org/datasets/catalog/scene_parse150" />
  <meta itemprop="sameAs" content="http://sceneparsing.csail.mit.edu/" />
  <meta itemprop="citation" content="&#10;@inproceedings{zhou2017scene,&#10;title={Scene Parsing through ADE20K Dataset},&#10;author={Zhou, Bolei and Zhao, Hang and Puig, Xavier and Fidler, Sanja and Barriuso, Adela and Torralba, Antonio},&#10;booktitle={Proceedings of the IEEE Conference on Computer Vision and Pattern Recognition},&#10;year={2017}&#10;}&#10;" />
</div>

# `scene_parse150`

Scene parsing is to segment and parse an image into different image regions
associated with semantic categories, such as sky, road, person, and bed. MIT
Scene Parsing Benchmark (SceneParse150) provides a standard training and
evaluation platform for the algorithms of scene parsing.

*   URL:
    [http://sceneparsing.csail.mit.edu/](http://sceneparsing.csail.mit.edu/)
*   `DatasetBuilder`:
    [`tfds.image.scene_parse_150.SceneParse150`](https://github.com/tensorflow/datasets/tree/master/tensorflow_datasets/image/scene_parse_150.py)
*   Version: `v1.0.0`
*   Versions:

    *   **`1.0.0`** (default):

*   Size: `936.97 MiB`

## Features
```python
FeaturesDict({
    'annotation': Image(shape=(None, None, 3), dtype=tf.uint8),
    'image': Image(shape=(None, None, 3), dtype=tf.uint8),
})
```

## Statistics

Split | Examples
:---- | -------:
ALL   | 22,210
TRAIN | 20,210
TEST  | 2,000

## Urls

*   [http://sceneparsing.csail.mit.edu/](http://sceneparsing.csail.mit.edu/)

## Supervised keys (for `as_supervised=True`)
`(u'image', u'annotation')`

## Citation
```
@inproceedings{zhou2017scene,
title={Scene Parsing through ADE20K Dataset},
author={Zhou, Bolei and Zhao, Hang and Puig, Xavier and Fidler, Sanja and Barriuso, Adela and Torralba, Antonio},
booktitle={Proceedings of the IEEE Conference on Computer Vision and Pattern Recognition},
year={2017}
}
```

--------------------------------------------------------------------------------
