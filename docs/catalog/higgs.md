<div itemscope itemtype="http://schema.org/Dataset">
  <div itemscope itemprop="includedInDataCatalog" itemtype="http://schema.org/DataCatalog">
    <meta itemprop="name" content="TensorFlow Datasets" />
  </div>

  <meta itemprop="name" content="higgs" />
  <meta itemprop="description" content="The data has been produced using Monte Carlo simulations. &#10;The first 21 features (columns 2-22) are kinematic properties &#10;measured by the particle detectors in the accelerator. &#10;The last seven features are functions of the first 21 features; &#10;these are high-level features derived by physicists to help &#10;discriminate between the two classes. There is an interest &#10;in using deep learning methods to obviate the need for physicists &#10;to manually develop such features. Benchmark results using &#10;Bayesian Decision Trees from a standard physics package and &#10;5-layer neural networks are presented in the original paper. &#10;&#10;&#10;To use this dataset:&#10;&#10;```python&#10;import tensorflow_datasets as tfds&#10;&#10;ds = tfds.load('higgs', split='train')&#10;for ex in ds.take(4):&#10;  print(ex)&#10;```&#10;&#10;See [the guide](https://www.tensorflow.org/datasets/overview) for more&#10;informations on [tensorflow_datasets](https://www.tensorflow.org/datasets).&#10;&#10;" />
  <meta itemprop="url" content="https://www.tensorflow.org/datasets/catalog/higgs" />
  <meta itemprop="sameAs" content="https://archive.ics.uci.edu/ml/datasets/HIGGS" />
  <meta itemprop="citation" content="@article{Baldi:2014kfa,&#10;      author         = &quot;Baldi, Pierre and Sadowski, Peter and Whiteson, Daniel&quot;,&#10;      title          = &quot;{Searching for Exotic Particles in High-Energy Physics&#10;                        with Deep Learning}&quot;,&#10;      journal        = &quot;Nature Commun.&quot;,&#10;      volume         = &quot;5&quot;,&#10;      year           = &quot;2014&quot;,&#10;      pages          = &quot;4308&quot;,&#10;      doi            = &quot;10.1038/ncomms5308&quot;,&#10;      eprint         = &quot;1402.4735&quot;,&#10;      archivePrefix  = &quot;arXiv&quot;,&#10;      primaryClass   = &quot;hep-ph&quot;,&#10;      SLACcitation   = &quot;%%CITATION = ARXIV:1402.4735;%%&quot;&#10;}&#10;" />
</div>

# `higgs`

The data has been produced using Monte Carlo simulations. The first 21 features
(columns 2-22) are kinematic properties measured by the particle detectors in
the accelerator. The last seven features are functions of the first 21 features;
these are high-level features derived by physicists to help discriminate between
the two classes. There is an interest in using deep learning methods to obviate
the need for physicists to manually develop such features. Benchmark results
using Bayesian Decision Trees from a standard physics package and 5-layer neural
networks are presented in the original paper.

*   URL:
    [https://archive.ics.uci.edu/ml/datasets/HIGGS](https://archive.ics.uci.edu/ml/datasets/HIGGS)
*   `DatasetBuilder`:
    [`tfds.structured.higgs.Higgs`](https://github.com/tensorflow/datasets/tree/master/tensorflow_datasets/structured/higgs.py)
*   Version: `v1.0.0`
*   Versions:

    *   **`1.0.0`** (default):
    *   `2.0.0`: New split API (https://tensorflow.org/datasets/splits)

*   Size: `2.62 GiB`

## Features
```python
FeaturesDict({
    'class_label': Tensor(shape=(), dtype=tf.float32),
    'jet_1_b-tag': Tensor(shape=(), dtype=tf.float64),
    'jet_1_eta': Tensor(shape=(), dtype=tf.float64),
    'jet_1_phi': Tensor(shape=(), dtype=tf.float64),
    'jet_1_pt': Tensor(shape=(), dtype=tf.float64),
    'jet_2_b-tag': Tensor(shape=(), dtype=tf.float64),
    'jet_2_eta': Tensor(shape=(), dtype=tf.float64),
    'jet_2_phi': Tensor(shape=(), dtype=tf.float64),
    'jet_2_pt': Tensor(shape=(), dtype=tf.float64),
    'jet_3_b-tag': Tensor(shape=(), dtype=tf.float64),
    'jet_3_eta': Tensor(shape=(), dtype=tf.float64),
    'jet_3_phi': Tensor(shape=(), dtype=tf.float64),
    'jet_3_pt': Tensor(shape=(), dtype=tf.float64),
    'jet_4_b-tag': Tensor(shape=(), dtype=tf.float64),
    'jet_4_eta': Tensor(shape=(), dtype=tf.float64),
    'jet_4_phi': Tensor(shape=(), dtype=tf.float64),
    'jet_4_pt': Tensor(shape=(), dtype=tf.float64),
    'lepton_eta': Tensor(shape=(), dtype=tf.float64),
    'lepton_pT': Tensor(shape=(), dtype=tf.float64),
    'lepton_phi': Tensor(shape=(), dtype=tf.float64),
    'm_bb': Tensor(shape=(), dtype=tf.float64),
    'm_jj': Tensor(shape=(), dtype=tf.float64),
    'm_jjj': Tensor(shape=(), dtype=tf.float64),
    'm_jlv': Tensor(shape=(), dtype=tf.float64),
    'm_lv': Tensor(shape=(), dtype=tf.float64),
    'm_wbb': Tensor(shape=(), dtype=tf.float64),
    'm_wwbb': Tensor(shape=(), dtype=tf.float64),
    'missing_energy_magnitude': Tensor(shape=(), dtype=tf.float64),
    'missing_energy_phi': Tensor(shape=(), dtype=tf.float64),
})
```

## Statistics

Split | Examples
:---- | ---------:
ALL   | 11,000,000
TRAIN | 11,000,000

## Urls

*   [https://archive.ics.uci.edu/ml/datasets/HIGGS](https://archive.ics.uci.edu/ml/datasets/HIGGS)

## Citation
```
@article{Baldi:2014kfa,
      author         = "Baldi, Pierre and Sadowski, Peter and Whiteson, Daniel",
      title          = "{Searching for Exotic Particles in High-Energy Physics
                        with Deep Learning}",
      journal        = "Nature Commun.",
      volume         = "5",
      year           = "2014",
      pages          = "4308",
      doi            = "10.1038/ncomms5308",
      eprint         = "1402.4735",
      archivePrefix  = "arXiv",
      primaryClass   = "hep-ph",
      SLACcitation   = "%%CITATION = ARXIV:1402.4735;%%"
}
```

--------------------------------------------------------------------------------
