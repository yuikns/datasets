<div itemscope itemtype="http://schema.org/Dataset">
  <div itemscope itemprop="includedInDataCatalog" itemtype="http://schema.org/DataCatalog">
    <meta itemprop="name" content="TensorFlow Datasets" />
  </div>

  <meta itemprop="name" content="squad" />
  <meta itemprop="description" content="Stanford Question Answering Dataset (SQuAD) is a reading comprehension dataset, consisting of questions posed by crowdworkers on a set of Wikipedia articles, where the answer to every question is a segment of text, or span, from the corresponding reading passage, or the question might be unanswerable.&#10;&#10;&#10;To use this dataset:&#10;&#10;```python&#10;import tensorflow_datasets as tfds&#10;&#10;ds = tfds.load('squad', split='train')&#10;for ex in ds.take(4):&#10;  print(ex)&#10;```&#10;&#10;See [the guide](https://www.tensorflow.org/datasets/overview) for more&#10;informations on [tensorflow_datasets](https://www.tensorflow.org/datasets).&#10;&#10;" />
  <meta itemprop="url" content="https://www.tensorflow.org/datasets/catalog/squad" />
  <meta itemprop="sameAs" content="https://rajpurkar.github.io/SQuAD-explorer/" />
  <meta itemprop="citation" content="@article{2016arXiv160605250R,&#10;       author = {{Rajpurkar}, Pranav and {Zhang}, Jian and {Lopyrev},&#10;                 Konstantin and {Liang}, Percy},&#10;        title = &quot;{SQuAD: 100,000+ Questions for Machine Comprehension of Text}&quot;,&#10;      journal = {arXiv e-prints},&#10;         year = 2016,&#10;          eid = {arXiv:1606.05250},&#10;        pages = {arXiv:1606.05250},&#10;archivePrefix = {arXiv},&#10;       eprint = {1606.05250},&#10;}&#10;" />
</div>

# `squad`

Stanford Question Answering Dataset (SQuAD) is a reading comprehension dataset,
consisting of questions posed by crowdworkers on a set of Wikipedia articles,
where the answer to every question is a segment of text, or span, from the
corresponding reading passage, or the question might be unanswerable.

*   URL:
    [https://rajpurkar.github.io/SQuAD-explorer/](https://rajpurkar.github.io/SQuAD-explorer/)
*   `DatasetBuilder`:
    [`tfds.text.squad.Squad`](https://github.com/tensorflow/datasets/tree/master/tensorflow_datasets/text/squad.py)

`squad` is configured with `tfds.text.squad.SquadConfig` and has the following
configurations predefined (defaults to the first one):

*   `plain_text` (`v0.1.0`) (`Size: 33.51 MiB`): Plain text

## `squad/plain_text`
Plain text

Versions:

*   **`0.1.0`** (default):
*   `1.0.0`: New split API (https://tensorflow.org/datasets/splits)

### Statistics

Split      | Examples
:--------- | -------:
ALL        | 98,169
TRAIN      | 87,599
VALIDATION | 10,570

### Features
```python
FeaturesDict({
    'answers': Sequence({
        'answer_start': Tensor(shape=(), dtype=tf.int32),
        'text': Text(shape=(), dtype=tf.string),
    }),
    'context': Text(shape=(), dtype=tf.string),
    'id': Tensor(shape=(), dtype=tf.string),
    'question': Text(shape=(), dtype=tf.string),
    'title': Text(shape=(), dtype=tf.string),
})
```

### Urls

*   [https://rajpurkar.github.io/SQuAD-explorer/](https://rajpurkar.github.io/SQuAD-explorer/)

## Citation
```
@article{2016arXiv160605250R,
       author = {{Rajpurkar}, Pranav and {Zhang}, Jian and {Lopyrev},
                 Konstantin and {Liang}, Percy},
        title = "{SQuAD: 100,000+ Questions for Machine Comprehension of Text}",
      journal = {arXiv e-prints},
         year = 2016,
          eid = {arXiv:1606.05250},
        pages = {arXiv:1606.05250},
archivePrefix = {arXiv},
       eprint = {1606.05250},
}
```

--------------------------------------------------------------------------------
