# 一些Python相关的学习笔记 #
***

## 1.Anaconda命令  
Anaconda入门网址：[http://docs.anaconda.com/anaconda/user-guide/getting-started/](http://docs.anaconda.com/anaconda/user-guide/getting-started/)

- 查看Anaconda内置的包和Python版本的方法
`conda list`、`python -V`

## 2.Python库的调用
- 各种python库的存放位置，可以从Github下载可用的库，然后放着路径即可调用。如`E:\ofAnaconda\Lib\site-packages\`
- **注意：有时候用pip已经安装好的包，在python仍然导入不了？**  
去`E:\ofAnaconda\Lib\site-packages\`把包复制到`E:\ofPython\ofInstallPython\Lib`中即可，或者可以在python中添加搜索路径`sys.path.append(r' ')`  

## 3.Linux install Anaconda
参考网址：[https://www.jianshu.com/p/f7c341085746](https://www.jianshu.com/p/f7c341085746)  
- 解决中文注释无法编译的问题: `# -*- coding: utf-8 -*-`  
## 4.常用python库的安装方法  
**总结：先用anaconda安装法，没装好再用pip安装，有时候安装失败是网络卡了，多试几次，或者修改pip的镜像服务器**  
例如链接到清华大学的镜像服务器[https://mirrors.tuna.tsinghua.edu.cn/](https://mirrors.tuna.tsinghua.edu.cn/),
>  找到python安装目录下的：`\Lib\site-packages\pip\models\index.py`文件，并将PYPI的值改为所需要的源网址  
`#PyPI = Index('https://pypi.python.org/')`  
`PyPI = Index('https://mirrors.tuna.tsinghua.edu.cn/') `   
![111.jpg](https://upload-images.jianshu.io/upload_images/18891803-32fd90447a5ca0ea.jpg?imageMogr2/auto-orient/strip%7CimageView2/2/h/300/w/400)
## 5.常用python库的安装方法  
**pip安装**  
1. conda list //查看已安装好的库  
2. pip install 库名  
3. pip install 库名 --upgrade  

**conda安装**  
1. conda install 库名  
2. conda update 库名   
3. conda update --all  *更新所有库*  
4. conda update conda  *更新 conda 自身*  
5. conda update anaconda  *更新 anaconda 自身*  
6. *直接用conda也适合没有安装pip的Linux系统*  

**其它**  
>- 要安装最新版本的“SomeProject”：  
pip install "SomeProject"  
>- 要安装特定版本：  
pip install "SomeProject==1.4"  
>- 要安装大于或等于一个版本而不是另一个版本：  
pip install "SomeProject>=1,<2"  
>- 安装一个版本 与某个版本 “兼容”： 
pip install "SomeProject~=1.4.2",*在这种情况下，这意味着安装任何版本“== 1.4。*”版本也是“> = 1.4.2”*  
>- 将已安装的SomeProject从PyPI 升级到最新版本。  
pip install --upgrade SomeProject  

**注：Anaconda常用python库：先安装Theano在安装Pymc3，不然pymc3装不上。**  
