# 使用介绍

## 工具

### apk tool

[相关地址](https://ibotpeaches.github.io/Apktool)

[配置方法](https://ibotpeaches.github.io/Apktool/install/)

### dex2jar 

[相关地址](https://sourceforge.net/projects/dex2jar/files/)

配置方法

* 解压缩 dex2jar-2.1.zip
* sudo mv /dex2jar-2.1  /usr/local/bin/
* sudo ln -s /usr/local/bin/dex2jar-2.1/d2j-dex2jar.sh /usr/local/bin/dex2jar
* sudo chmod +x /usr/local/bin/dex2jar


### jd-gui

[相关地址](https://github.com/java-decompiler/jd-gui)
* 解压缩 jd-gui.zip， 生成jd-gui文件夹
* sudo mv jd-gui /usr/local/bin/
* sudo ln -s /usr/local/bin/jd-gui/jd-gui.sh /usr/local/bin/jdgui
* sudo chmod +x /usr/local/bin/jdgui
* 修改/usr/local/bin/jd-gui/jd-gui.sh文件中JAVA_HOME的配置为你的配置

## 使用

apktool 工具主要用来查看资源

* apktool d   xxx.apk    //解压缩apk, 解出资源文件, 以及smali代码
* apktool b  xxx/           //生成apk, 位置在 xxx/build

dex2jar 与 jd-gui配置查看代码逻辑

* dex2jar xxx.dex    //将dex转化成jar文件
* jd-gui  //打开生成的jar文件

