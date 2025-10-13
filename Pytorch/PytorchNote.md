# Pytorch!启动！

## 库的导入与功能
- `import torch`
  > 张量，神经网络层，自动求导等
- `import matplotlib.pyplot as plt`
  > 绘图库，用于数据可视化
- `import numpy as np`
  > 数值计算库，提供数组操作、数学函数
- `from torchvision import datasets`
  >包含常用数据集
- `from torchvision import transform`
  > 数据预处理工具，缩放、裁剪、转张量

### 1.torch  
- `torch._version_`
  >torch版本
- `torch._file_`
  >torch路径

### 2.matplotlib.pyplot(plt)  
- `plt.plot([1,2,3,4])`
- `plt.ylabel('temperature')`
- `plt.show()`
- ~~`plt.imshow()`~~
- `plt.title('标题')`
- `plt.ylabel('Y轴')`
- `plt.xlabel('X轴')`

### 3.transforms(from torchvision)
- `transforms.ToTensor()`
  >构造数据转换器

### 4.datasets(from torchvision)
- `train_data = datasets.MNISt(root='./当前文件夹下的data文件夹' , train=Ture , download=True , transform=转换器)`
  - root：根目录
  - train: 导入训练集与否
  - download: 本地/线上下载
  - transform: 用一个转化器处理数据





















