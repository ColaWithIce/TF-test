# TF-test
ipython notebook

DCGANCopy1.ipynb:

net = slim.conv2d(net, 64, [4, 4], 2, normalizer_fn=None, activation_fn=None, biases_initializer=None, reuse=reuse)

output1 = slim.batch_norm(net)


DCGAN.ipynb:

output2 = slim.conv2d(net, 64 ,[4, 4], 2, normalizer_fn=slim.batch_norm, activation_fn=None, reuse=reuse)

