# TF-test
ipython notebook

@mikowals @girving Actually, I read the [code]( https://github.com/tensorflow/tensorflow/blob/r0.11/tensorflow/contrib/layers/python/layers/layers.py), from line 439 to 455, it describes how the conv2d layer uses the batch_norm and activation. What I understand from this is that the `reuse` parameter only influnence the `conv2d` layer but not the function used inside.
To make the two ways same, I also set `biases_initializer` None.

@girving I just try one [tutorial](https://github.com/awjuliani/TF-Tutorials/blob/master/DCGAN.ipynb) written by @awjuliani. Here are the two ways I used in the code which I use Ipython notebook to test. What I just change is the `dis3` of the `discriminator`. The first way ipython notebook is shown here. The second is here. The output of the training message is very different. The two way's result should be similar but now as you can see the Disc Loss are not in same scale. I just wonder why this will happen. Is there something wrong with the variable updating or the way I use the code is wrong. 
