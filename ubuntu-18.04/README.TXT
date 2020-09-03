基于官网ubuntu:18.04建造一个尽量小的docker image.

建造思路：

1 启动image
2 apt安装必要的包
3 dcoker diff查看并记录安装了那些文件 --> 存放在diff文件里
4 把这些文件复制到宿主机上
5 保存一个更新的image
6 用新的image重复第一步
