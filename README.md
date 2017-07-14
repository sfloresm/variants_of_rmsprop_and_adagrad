# Variants of Adagrad and RMSProp

Keras implementation of SC-Adagrad, SC-RMSProp and RMSProp Algorithms proposed in [here](https://arxiv.org/abs/1706.05507)

Short version accepted at ICML, 17 can be found [here](http://www.ml.uni-saarland.de/Publications/MukHei-VariantsRMSPropAdagradLogRegret.pdf)

I wrote a blog [here](https://mmahesh.github.io/articles/2017-07/tutorial-on-sc-adagrad-a-new-stochastic-gradient-method-for-deep-learning) describing the algorithms in simple terms so that it is easy to understand the gist of the algorithms.


# Usage

So, you created a network, now you want to train with above algorithms. Copy the file into new_optimizers.py into your repository

```python
from new_optimizers.py import *

# lets for example you want to use SC-Adagrad then
# create optimizer object as follows.

sc_adagrad = SC_Adagrad()
```

Then in the code where you compile your model you must set 'optimizer=sc_adagrad'. You can do the same for SC-RMSProp and RMSProp algorithms.

## I hope this is helpful :).
