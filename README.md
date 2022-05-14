# Shell
主要写一些平时积累的命令行，不确定时间更新

# file path & file name
不含后缀带路径的文件名:
```
filename = os.path.splitext(filepath)[0]
```
后缀:
```
filename = os.path.splitext(filepath)[-1]
```
带后缀的文件名:
```
filename = os.path.basename(filepath)
```
不带后缀的文件名,对于filepath2这种情况不适合，从第一个点开始后面的都会被去掉:
```
filename= filename.split('.')[0]
```

# Environment

Python 3.9.0

Tensorflow 2.5.0rc1

# pip & conda

# gpustat
install
```
pip install gpustat
```
可以提供更美观简洁的展示，结合watch命令，可以动态实时监控GPU的使用情况。
```
watch --color -n1 gpustat -cpu
```
# 国内镜像源
[清华](https://pypi.tuna.tsinghua.edu.cn/simple) https://pypi.tuna.tsinghua.edu.cn/simple

[阿里云](http://mirrors.aliyun.com/pypi/simple/) http://mirrors.aliyun.com/pypi/simple/

[中国科技大学](https://pypi.mirrors.ustc.edu.cn/simple/) https://pypi.mirrors.ustc.edu.cn/simple/

[华中理工大学](http://pypi.hustunique.com/) http://pypi.hustunique.com/

[山东理工大学](http://pypi.sdutlinux.org/) http://pypi.sdutlinux.org/

[豆瓣](http://pypi.douban.com/simple/) http://pypi.douban.com/simple/

Linux下，修改 ~/.pip/pip.conf (没有就创建一个文件夹及文件。文件夹要加“.”，表示是隐藏文件夹),内容如下：
```
[global]
index-url = https://pypi.tuna.tsinghua.edu.cn/simple
[install]
trusted-host=mirrors.aliyun.com
```
windows下，直接在user目录中创建一个pip目录，再新建文件pip.ini。（例如：C:\Users\WQP\pip\pip.ini）内容同上。

# Reference

[[1] Cross Stage Partial Network (CSPNet)](https://arxiv.org/pdf/1911.11929.pdf)
