# Deep Learning For Folks Without (or With!) a Ph.D

Speaker: Douglass Starnes

Repo: https://github.com/douglasstarnes/pytn2019
Slides:

## Machine learning in 7 steps
acquire, clean, split
train, test, score
evaluate

## mnist dataset

60k hand written digits

Step 1: Acquire

```
from tensorflow.examples.tutorials.mnist import input_data
mnist = input_data.read_data_sets('MNIST_data', one_hot=True)
```

Step 2: (Data is already clean.)

Step 3: (Data is already split.)

```
print(mnist.train.num_examples)
55000

print(mnist.test.num_examples)
10000
```

Step 4: Train

```
x = tf.placeholder(tf.float32, shape=[None, 784])  #input for feature vectors
y_hat = tf.placeholder(tf.float32, shape=[None, 10])  #input for targets
weights = tf.Variable(tf.zeros([784,10]))  #initialize model with random values
bias = tf.Variable(tf.zeros([10]))

optimizer = tf.train.GradientDescentOptimizer(0.5).minimize(cost_function)

with tf.Session() as sess:
    sess.run(tf.global_variables_initializer())
    for _ in mnist.train.num_examples / 100: # run one epoch
        batch = mnist.train.next_batch(100)
        sess.run(optimizer, feed_dict={x: batch[0], y_hat: batch[1]})

```

## Keras

Keras is a wrapper around Tensorflow. If you have a problem and you want to solve it, you used Keras.

You define they type of model you are using. In our example it is Sequential...

``` from keras.models import Sequential```




