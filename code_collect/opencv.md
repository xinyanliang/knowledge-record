- [opencv document](http://docs.opencv.org/3.0-beta/doc/py_tutorials/py_gui/py_image_display/py_image_display.html)


- opencv install

```
pip install opencv-python
```

opencv 使用多维的numpy数组表示RGB图像，但是顺序是反的，即<font color='red'>BGR</font>.我们可以使用下面的代码从 __BGR__ 转到 __RGB__：
```
cv2.cvtColor(image, cv2.COLOR_BGR2RGB)
```
