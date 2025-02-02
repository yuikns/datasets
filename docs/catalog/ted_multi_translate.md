<div itemscope itemtype="http://schema.org/Dataset">
  <div itemscope itemprop="includedInDataCatalog" itemtype="http://schema.org/DataCatalog">
    <meta itemprop="name" content="TensorFlow Datasets" />
  </div>

  <meta itemprop="name" content="ted_multi_translate" />
  <meta itemprop="description" content="Massively multilingual (60 language) data set derived from TED Talk transcripts.&#10;Each record consists of parallel arrays of language and text. Missing and&#10;incomplete translations will be filtered out.&#10;&#10;&#10;To use this dataset:&#10;&#10;```python&#10;import tensorflow_datasets as tfds&#10;&#10;ds = tfds.load('ted_multi_translate', split='train')&#10;for ex in ds.take(4):&#10;  print(ex)&#10;```&#10;&#10;See [the guide](https://www.tensorflow.org/datasets/overview) for more&#10;informations on [tensorflow_datasets](https://www.tensorflow.org/datasets).&#10;&#10;" />
  <meta itemprop="url" content="https://www.tensorflow.org/datasets/catalog/ted_multi_translate" />
  <meta itemprop="sameAs" content="https://github.com/neulab/word-embeddings-for-nmt" />
  <meta itemprop="citation" content="@InProceedings{qi-EtAl:2018:N18-2,&#10;  author    = {Qi, Ye  and  Sachan, Devendra  and  Felix, Matthieu  and  Padmanabhan, Sarguna  and  Neubig, Graham},&#10;  title     = {When and Why Are Pre-Trained Word Embeddings Useful for Neural Machine Translation?},&#10;  booktitle = {Proceedings of the 2018 Conference of the North American Chapter of the Association for Computational Linguistics: Human Language Technologies, Volume 2 (Short Papers)},&#10;  month     = {June},&#10;  year      = {2018},&#10;  address   = {New Orleans, Louisiana},&#10;  publisher = {Association for Computational Linguistics},&#10;  pages     = {529--535},&#10;  abstract  = {The performance of Neural Machine Translation (NMT) systems often suffers in low-resource scenarios where sufficiently large-scale parallel corpora cannot be obtained. Pre-trained word embeddings have proven to be invaluable for improving performance in natural language analysis tasks, which often suffer from paucity of data. However, their utility for NMT has not been extensively explored. In this work, we perform five sets of experiments that analyze when we can expect pre-trained word embeddings to help in NMT tasks. We show that such embeddings can be surprisingly effective in some cases -- providing gains of up to 20 BLEU points in the most favorable setting.},&#10;  url       = {http://www.aclweb.org/anthology/N18-2084}&#10;}&#10;" />
</div>

# `ted_multi_translate`

Massively multilingual (60 language) data set derived from TED Talk transcripts.
Each record consists of parallel arrays of language and text. Missing and
incomplete translations will be filtered out.

*   URL:
    [https://github.com/neulab/word-embeddings-for-nmt](https://github.com/neulab/word-embeddings-for-nmt)
*   `DatasetBuilder`:
    [`tfds.translate.ted_multi.TedMultiTranslate`](https://github.com/tensorflow/datasets/tree/master/tensorflow_datasets/translate/ted_multi.py)

`ted_multi_translate` is configured with
`tfds.core.dataset_builder.BuilderConfig` and has the following configurations
predefined (defaults to the first one):

*   `plain_text` (`v0.0.3`) (`Size: 335.91 MiB`): Plain text import of
    multilingual TED talk translations

## `ted_multi_translate/plain_text`
Plain text import of multilingual TED talk translations

Versions:

*   **`0.0.3`** (default):
*   `1.0.0`: New split API (https://tensorflow.org/datasets/splits)

### Statistics

Split      | Examples
:--------- | -------:
ALL        | 271,360
TRAIN      | 258,098
TEST       | 7,213
VALIDATION | 6,049

### Features
```python
FeaturesDict({
    'talk_name': Text(shape=(), dtype=tf.string),
    'translations': TranslationVariableLanguages({
        'language': Text(shape=(), dtype=tf.string),
        'translation': Text(shape=(), dtype=tf.string),
    }),
})
```

### Urls

*   [https://github.com/neulab/word-embeddings-for-nmt](https://github.com/neulab/word-embeddings-for-nmt)

## Citation
```
@InProceedings{qi-EtAl:2018:N18-2,
  author    = {Qi, Ye  and  Sachan, Devendra  and  Felix, Matthieu  and  Padmanabhan, Sarguna  and  Neubig, Graham},
  title     = {When and Why Are Pre-Trained Word Embeddings Useful for Neural Machine Translation?},
  booktitle = {Proceedings of the 2018 Conference of the North American Chapter of the Association for Computational Linguistics: Human Language Technologies, Volume 2 (Short Papers)},
  month     = {June},
  year      = {2018},
  address   = {New Orleans, Louisiana},
  publisher = {Association for Computational Linguistics},
  pages     = {529--535},
  abstract  = {The performance of Neural Machine Translation (NMT) systems often suffers in low-resource scenarios where sufficiently large-scale parallel corpora cannot be obtained. Pre-trained word embeddings have proven to be invaluable for improving performance in natural language analysis tasks, which often suffer from paucity of data. However, their utility for NMT has not been extensively explored. In this work, we perform five sets of experiments that analyze when we can expect pre-trained word embeddings to help in NMT tasks. We show that such embeddings can be surprisingly effective in some cases -- providing gains of up to 20 BLEU points in the most favorable setting.},
  url       = {http://www.aclweb.org/anthology/N18-2084}
}
```

--------------------------------------------------------------------------------
