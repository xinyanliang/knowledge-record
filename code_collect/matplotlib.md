### [Matplotlib](http://matplotlib.org/)

### 如何用matplotlib画gif动图

[参考](https://eli.thegreenplace.net/2016/drawing-animated-gifs-with-matplotlib/)
[参考](https://stackoverflow.com/questions/23856990/cant-save-matplotlib-animation)

若想要用 matplotlib 的 <font color="red">save </font>方法渲染 GIF 动图的话，就必须安装 <font color="red"><b><a href="https://www.imagemagick.org/script/index.php">ImageMagick</a></b></font> 。

``` python
import numpy as  np
from matplotlib import pyplot as plt
from matplotlib.animation import FuncAnimation, FFMpegWriter
import seaborn as sns
sns.set()

fig , ax = plt.subplots()
fig.set_tight_layout(True)

#画出一个维持不变（不会被重画）的散点图和一开始的那条直线。
x = np.arange(0,20,0.1)
y = np.random.normal(0,3.0,len(x))
ax.scatter(x,y)
line, = ax.plot(x, x-5, '-r', linewidth=2)

def update(i):
    label = "timestep {0}".format(i)
    # 更新直线和x轴（用一个新的x轴的标签）。
    # 用元组（Tuple）的形式返回在这一帧要被重新绘图的物体
    line.set_ydata(x-5+i)
    ax.set_label(label)

    return line, ax

if __name__ == "__main__":
    # FuncAnimation 会在每一帧都调用“update” 函数。
    # 在这里设置一个10帧的动画，每帧之间间隔200毫秒
    anim = FuncAnimation(fig,update,frames=10,interval=200)
  
    ######## warm reminder #####################
    ##必须指定ffmpeg.exe的路径,否者报错“FileNotFoundError: [WinError 2] 系统找不到指定的文件。”
    plt.rcParams['animation.ffmpeg_path'] = 'C:\\ProgramData\\ffmpeg\\bin\\ffmpeg.exe'
    FFwriter = FFMpegWriter()
    anim.save('line.mp4', dpi=80,writer=FFwriter)
    plt.show()
```

### [彩色映射散点图](http://codingpy.com/article/a-quick-intro-to-matplotlib/)

``` python
import matplotlib.pyplot as plt
import numpy as np
x = np.random.rand(1000)
y = np.random.rand(1000)
size = np.random.rand(1000) * 50
colour = np.random.rand(1000)
plt.scatter(x, y, size, colour)
plt.colorbar()
plt.show()
```
