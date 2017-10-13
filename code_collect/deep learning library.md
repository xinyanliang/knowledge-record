### Keras以Tensorflow为后端， 指定GPU运行程序

[参考](http://www.bijishequ.com/detail/461561)
``` python
import os
#制定GPU 0, 1, 4
os.environ["CUDA_VISIBLE_DEVICES"] = "0,1,4"
````

### 通过制定种子使得代码结果重现
```
import numpy as np
from numpy.random import seed
seed(1)
from tensorflow import set_random_seed
set_random_seed(2)
```
