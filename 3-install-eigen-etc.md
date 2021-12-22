# 这个教程是安装SLAM十四讲中需要用到的依赖库（均为ubuntu16.04系统）
1. Eigen安装（必要的）  
安装方法：sudo apt install libeigen3-dev  
安装位置：Eigen是一个纯用头文件搭建起来的库（没有库文件），其头文件的默认位置在：/usr/include/eigen3
2. Pangolin安装（可选）  
安装方法：  
git clone https://github.com/stevenlovegrove/Pangolin.git   
cd Pangolin   
sudo apt install libgl1-mesa-dev libglew-dev cmake   
sudo apt install libpython2.7-dev python-pip    
git submodule init && git submodule update   
sudo python -mpip install numpy pyopengl Pillow pybind11   
sudo apt install pkg-config    
sudo apt install libegl1-mesa-dev libwayland-dev libxkbcommon-dev wayland-protocols    
mkdir build   
cd build      
cmake ..  
make   
sudo make install   
安装位置：   
头文件的默认位置在/usr/local/include/pango,库文件的默认位置在/usr/lib/x86_64-linux-gnu下      
3. Sophus安装（可选）  
安装方法：  
git clone https://github.com/strasdat/Sophus.git
cd [path-to-Sophus]
git checkout a621ff	# 将Sophus库切换到非模板类/双精度版本   
mkdir build   
cd build   
cmake ..                              
make                          # Sophus库只需编译无需安装（编译的build文件夹不可删除）
可能遇见的错误解决方案参考：https://github.com/uzh-rpg/rpg_svo/issues/237   
安装位置：   
头文件的默认位置在[path-to-Sophus]/sophus，库文件的默认位置在[path-to-Sophus]/build下，我们可找到名为libSophus.so的库文件。      
4. g2o(可选)   
安装方法：   
git clone https://github.com/RainerKuemmerle/g2o.git   
cd [path-to-g2o]
#dependencies   
sudo apt install cmake libeigen3-dev 
sudo apt install libsuitesparse-dev qtdeclarative5-dev qt5-qmake libqglviewer-dev
#building and installing   
mkdir build   
cd build   
cmake ..   
make -j12   
sudo make install   
安装位置：   
头文件的默认位置在/usr/local/include/g2o，库文件的默认位置在/usr/local/lib   