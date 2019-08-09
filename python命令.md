#  ipynb文件   
***  

##  1. 关于如何查看并运行.ipynb文件  
   1）原始查看可以用Anaconda附带的Spyder IDE框架，但没有层次感  
   2）在jupyter notebook上比较代码调理比较清晰  

**cmd中输入：`jupyter notebook`**  
- 先弹出的页面**upload**这个`.ipynb`后缀的文件，然后点击打开它  

![搜狗截图_2019-08-09_11-18-23.jpg](https://upload-images.jianshu.io/upload_images/18891803-249c7262cd73de7f.jpg?imageMogr2/auto-orient/strip%7CimageView2/2/h/300/w/400)  

**下一页可进行运行和另存为.py文件**  
![搜狗截图_2019-08-09_11-18-59.jpg](https://upload-images.jianshu.io/upload_images/18891803-d933b881fef0eddc.jpg?imageMogr2/auto-orient/strip%7CimageView2/2/h/300/w/400)  

##  2. 关于如何将.ipynb文件转换为.py文件  
转的demo.ipynb所在目录下，打开终端（shift+鼠标右键），然后输入命令：    
`jupyter nbconvert --to script targetfile.ipynb`  
或者  
`jupyter nbconvert --to python targetfile.ipynb` 
