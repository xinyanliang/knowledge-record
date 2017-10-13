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

### Below program loads an image in grayscale, displays it, save the image if you press ‘s’ and exit, or simply exit without saving if you press ESC key.
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
