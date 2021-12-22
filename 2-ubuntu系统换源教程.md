# ubuntu系统换源教程

为什么换源？Ubuntu系统原装的源都是国外的源，因此在更新软件时，网速会特别的慢，因此需要将源改为国内源，  
加快安装、下载速度。

**博客教程**
https://blog.csdn.net/m0_46378002/article/details/107697231

**arm架构系统换源**
1. 先将以前的源备份  
命令：sudo cp /etc/apt/sources.list /etc/apt/sources.list.old
2. 然后打开源文件  
命令：sudo gedit /etc/apt/sources.list  
将打开的文件里面的内容更改为以下内容  
3. 选择国内源（**注意选择ubuntu系统以及系统架构**）   
清华源网址：https://mirrors.tuna.tsinghua.edu.cn/help/ubuntu/  
中科大源网址：https://mirrors.ustc.edu.cn/repogen/  
阿里云源：https://developer.aliyun.com/mirror/  
4. 切换源  
将源内容替换，使用sudo apt-get update 更新即可。  

**amd架构系统换源**
1. 先将以前的源备份  
命令：sudo cp /etc/apt/sources.list /etc/apt/sources.list.old
2. 然后打开源文件  
命令：sudo gedit /etc/apt/sources.list  
将打开的文件里面的内容更改为以下内容  
3. 选择国内源（**注意选择ubuntu系统以及系统架构**）   
清华源网址：https://mirrors.tuna.tsinghua.edu.cn/help/ubuntu/  
中科大源网址：https://mirrors.ustc.edu.cn/repogen/  
阿里云源：https://developer.aliyun.com/mirror/  
4. 切换源  
将源内容替换，使用sudo apt-get update 更新即可。  