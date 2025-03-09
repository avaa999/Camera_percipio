# Camera_percipio
图漾相机的使用记录
## 目录
- [安装驱动](#安装驱动) <br>
参考官网：https://doc.percipio.xyz/cam/latest/getstarted/sdk-python-linux-compile.html#linux-python-label ；<br>
注意由make生成的动态链接库，其路径为/usr/local/pcammls/PYTHON，在该路径下可以直接运行 python3 frame_frtch.py；PS：如果要在其它工程中运行相应功能的.py文件，则需要拷贝动态链接库，代码如下：<br>
`` sudo cp libtycam.so.3.6.66 /home/liuaohua/camport_multi_language-master/python/``
注意上述代码要在``/usr/local/pcammls/PYTHON``路径下打开终端执行，``libtycam.so.3.6.66``为动态链接库相关的文件，``/home/liuaohua/camport_multi_language-master/python/``为你的工程
- [基于颜色的特征点动态检测](#基于颜色的特征点动态检测)
- [相机外惨标定](#相机外惨标定)
获取相机到机械臂基座标的变换矩阵
