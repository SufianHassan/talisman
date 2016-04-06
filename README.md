[![Build Status](https://travis-ci.org/Yomguithereal/talisman.svg)](https://travis-ci.org/Yomguithereal/talisman)

# Talisman

[Full documentation](http://yomguithereal.github.io/talisman/)

Talisman is a JavaScript library collecting series of algorithms related to the three following domains:

* [Fuzzy logic & fuzzy matching](https://en.wikipedia.org/wiki/Approximate_string_matching)
* [Natural Language Processing (NLP)](https://en.wikipedia.org/wiki/Natural_language_processing)
* [Machine learning](https://en.wikipedia.org/wiki/Machine_learning)

## Installation

You can install **Talisman** through npm:

```bash
npm install talisman
```

## Documentation

The library's full documentation can be found [here](http://yomguithereal.github.io/talisman/).

## Goals

* **Modular**: the library is completely modular. This means that if you only need to compute a `levenshtein` distance, you will only load the relevant code.
* **Straightfoward & simple**: just want to compute a jaccard index? No need to instantiate a class and use two methods to pass options and then finally succeed in getting the index. Just apply the `jaccard` function and get going.
* **Consistent API**: the library's API is fully consistent and one should not struggle to understand how to apply two different distance metrics.
* **Functional**: except for cases where classes might be useful (classifiers notably), *Talisman* only uses functions, only consumes raw data and will order functions' arguments to make partial application & currying etc. as easy as possible.
* **Performant**: the library should be as performant as possible for a high-level programming language library.
* **Cross-platform**: the library is cross-platform and can be used both on node.js and in the browser.

## Contribution

Contributions are of course welcome :)

Be sure to lint & pass the unit tests before submitting your pull request.

```bash
# Cloning the repo
git clone git@github.com:Yomguithereal/talisman.git
cd talisman

# Installing the deps
npm install

# Running the tests
npm test

# Linting the code
npm run lint
```

## Current modules

* clustering
  * k-means
* helpers
  * vectors
* metrics
  * cosine
  * dice
  * euclidean
  * hamming
  * jaccard
  * jaro
  * jaro-winkler
  * levenshtein
  * manhattan
  * mra
  * overlap
  * sorensen
  * tversky
* phonetics
  * caverphone
  * cologne
  * doubleMetaphone
  * metaphone
  * mra
  * nysiis
  * soundex
* regex
  * classes
* stats
  * frequencies
  * ngrams
  * tfidf
* stemmers
  * lancaster
  * lovins
  * porter
  * latin
    * schinke
* tokenizers
  * sentences
    * naive
  * words
    * naive
    * treebank

## License

[MIT](./LICENSE.txt)
