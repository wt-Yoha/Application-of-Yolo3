原项目来自：https://github.com/qqwweee/keras-yolo3
测试图片集来自：https://github.com/experiencor/kangaroo

对原项目训练方法进行了补充：
1 编辑classes.txt文件 加入自己需要分类的目标
2 生成annotation.txt文件 格式为 path\\image.jpg xmin,ymin,xmax,ymax,id (next box)
3 确保有预训练的权重文件
4 修改train.py 中的classes、annotation文件为第1步中的
5 运行train.py 生成的log文件夹中的trained_weights_final.h5 即为训练结果
6 修改yolo_video.py中的classes和xxx.h5权重文件并运行
