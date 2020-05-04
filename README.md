# Probe-Masked-LMs
Since the Language Model BERT was released in 2018, NLP researchers have raised the question: Can we use BERT (and other models) as a knowledge base? (https://github.com/facebookresearch/LAMA)
Here is a short collection of Notebooks that let you quickly probe what different language models know about the world.

The common procedure is to formulate a probe by creating a simple sentence of the form "subject relation object". We then mask the object and pass that to the Language Model as "subject relation [MASK]".
Unfortunately there is are some annoying constraints with this simple approach, most importantly: The object you mask can only be a single token. So that means you can't ask for e.g. full names like "Albert Einstein" that easily.
