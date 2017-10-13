### Keras以Tensorflow为后端， 指定GPU运行程序

[参考](http://www.bijishequ.com/detail/461561)
``` python
import os
#指定程序在GPU 0, 1, 4运行
os.environ["CUDA_VISIBLE_DEVICES"] = "0,1,4"
````

### Keras通过Tensorflow实现GPU并行

[参考1](http://blog.csdn.net/u010159842/article/details/59104029)
[参考2](https://www.tensorflow.org/deploy/distributed)

### 通过制定种子使得代码结果重现
``` python
import numpy as np
from numpy.random import seed
seed(1)
from tensorflow import set_random_seed
set_random_seed(2)
```

### tensorflow的tensor与numpy的ndarray转化

``` python
import tensorflow as tf
# convert tensor into ndarray
tf.Session().run(tensor)
#convert ndarray into tensor
tf.convert_to_tensor(img.eval())
```
