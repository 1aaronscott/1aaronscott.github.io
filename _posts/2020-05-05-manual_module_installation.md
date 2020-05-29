---
layout: post
title: Manual Installation of a Python Module
subtitle: With SpaCy and Conda as an example
gh-repo: 1aaronscott
gh-badge: [star, fork, follow]
tags: [blog, nlp, python]
comments: true
image: ../img/spacy_logo.jpg
---
Sometimes you may need to manually install a python module. I had to do this because
the large SpaCy model at the time of wrting is almost 800 megabytes compressed (and close to 1 gigabyte
uncompressed) but module managers download temporarily to /tmp before installation.
My /tmp directory is not that large and really no /tmp really should have to be.

* Search for and download (to a location with plenty of space) the model from the [github release page](https://github.com/explosion/spacy-models/tags)
* Unpack the tarball with `tar xvzf [file]`
* `cd` into the newly created directory
* Activate your conda environment (e.g. `conda activate spacy-tryout`)
* Run a command similar to `python setup.py install` as appropriate for your system
* Some time will pass as there will be further unpacking and then installation
* When complete, you should be able to find the SpaCy install in your anaconda folder (e.g. `~/anaconda3/envs/spacy-tryout/lib/python3.7/site-packages`)
