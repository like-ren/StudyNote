# Pytorch!启动！

## 库的导入与功能
- `import torch`
  > 张量，神经网络层，自动求导等
- `import matplotlib.pyplot as plt`
  > 绘图库，用于数据可视化
- `import numpy as np`
  > 数值计算库，提供数组操作、数学函数
- `from torchvision import datasets`
  > 包含常用数据集
- `from torchvision import transform`
  > 数据预处理工具，缩放、裁剪、转张量

### 1.torch  
- `torch._version_`
  > torch版本
- `torch._file_`
  > torch路径
- `torch.utils.data.Dataloader(data,batch_size=64,shuffle=True)`
  > - data放要加载的数据  
  > - batch_size代表每批加载多少数据    
  > - shuffle代表是否打乱顺序  
  > - utils工具模块  data数据处理子模块  DataLoader数据加载器类  
  > - 数据加载器用于有规划地批量提供数据  
  > > `loader=torch.utils.data.Dataloader(traindata,batch_size=64,shuffle=True)`  
  > > 从traindata里面加载数据，每批64个，随机加载，存放到loader中  
  > > `images,labels=next(iter(loader))`  
  > > 用迭代器逐一读取数据，images存放图片，labels存放标签  
  > > `images.shape`      images的属性  
  > > `images[0]`          第一张图片  
  > > `images[23,0,12,13]`      第24张图片，0灰度层，13行14列的像素  

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
  >将原始数据转换为机器学习模型需要的小数，并转为pytorch需要的张量

### 4.datasets(from torchvision)
- `train_data = datasets.MNISt(root='./当前文件夹下的data文件夹' , train=Ture , download=True , transform=转换器)`
  - root：根目录
  - train: 导入训练集与否
  - download: 本地/线上下载
  - transform: 用一个转化器处理数据





















