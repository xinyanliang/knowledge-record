- [opencv document](http://docs.opencv.org/3.0-beta/doc/py_tutorials/py_gui/py_image_display/py_image_display.html)


- opencv install

```
pip install opencv-python
```

### opencv 使用多维的numpy数组表示RGB图像，但是顺序是反的，即<font color='red'>BGR</font>.我们可以使用下面的代码从 __BGR__ 转到 __RGB__：
``` python
cv2.cvtColor(image, cv2.COLOR_BGR2RGB)
```

### 显示一个图
``` python
cv2.imshow('image',img)
//必须加后面两行
cv2.waitKey(0)
cv2.destroyAllWindows()
```

### 以灰度图加载一个图，显示它，如果按s保存图并退出，按ESC键不保存退出.
``` python
import numpy as np
import cv2

img = cv2.imread('messi5.jpg',0)
cv2.imshow('image',img)
k = cv2.waitKey(0)
if k == 27:         # wait for ESC key to exit
    cv2.destroyAllWindows()
elif k == ord('s'): # wait for 's' key to save and exit
    cv2.imwrite('messigray.png',img)
    cv2.destroyAllWindows()
```

### 使用matplotlib
``` python
import numpy as np
import cv2
from matplotlib import pyplot as plt

img = cv2.imread('messi5.jpg',0)
plt.imshow(img, cmap = 'gray', interpolation = 'bicubic')
plt.xticks([]), plt.yticks([])  # to hide tick values on X and Y axis
plt.show()
```

## 读入视频

为了获取视频，应该创建一个 VideoCapture 对象。他的参数可以是设备的索引号，或者是一个视频文件。设备索引号就是在指定要使用的摄像头。
一般的笔记本电脑都有内置摄像头。所以参数就是 0。你可以通过设置成 1 或者其他的来选择别的摄像头。之后，你就可以一帧一帧的捕获视频了。但是最后，别忘了停止捕获视频。[ref](http://blog.csdn.net/qq_18343569/article/details/50275305)

```python
import cv2
import numpy as np

cap = cv2.VideoCapture('dM06AMFLsrc.mp4')

vid = []
while True:
    ret, img = cap.read()
    if not ret:
        break
    vid.append(cv2.resize(img, (171, 128)))
vid = np.array(vid, dtype=np.float32) 
```
