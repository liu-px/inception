# flower_world

这是一个图像识别项目，基于tensorflow，现有的CNN网络可以识别四种花的种类。适合新手对使用tensorflow进行一个完整的图像识别过程有一个大致轮廓。项目包括对数据集的处理，从硬盘读取数据，CNN网络的定义，训练过程，还实现了一个GUI界面用于使用训练好的网络。
## Require
1. Python3.5+
2. tensorflow
3. wxPython

## Quick start
- git clone这个项目
- 导入你喜欢的IDE如pycharm，或者你喜欢的编辑器如Atom。
- 解压input_data.rar到你喜欢的目录。
- 修改train.py中
```
train_dir = 'D:/xxxx/xxxxx/input_data'  # 训练样本的读入路径
logs_train_dir = 'D:/xxxx/xxxxx/save'  # logs存储路径
```
为你本机的目录。
- 运行train.py开始训练。
- 训练完成后，修改test.py中的`logs_train_dir = 'D:/xxxxxx/save/'`为你的目录。
- 运行test.py或者gui.py查看结果。

另外本项目分别有inception_resnet_v1, inceptionV1, inceptionV2 和 inceptionV4 四种网络模型，如果像训练某一个模型，可以在train.py文件中修改模型名称并训练，另外需注意的是因为原始图片的尺寸原因，所以模型并不是标准的。
