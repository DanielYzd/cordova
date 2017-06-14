# cordova
> cordova-安卓app打包工具

# 环境搭建
> 材料,准备工作

项目  | 验证安装完成 | 教程
------------ | -------------   | -------------
npm  |  npm -v | node自带
npm install -g cordova |  cordova -v |   [cordova打包教程](http://www.jianshu.com/p/60e98587ae89)
jdk  | javac（安装jdk主要是目录，推荐默认，会安装好jir跟jdk两个目录） |  [jdk安装](http://jingyan.baidu.com/article/bea41d435bc695b4c41be648.html)
sdk | adb这个也是需要配环境变量的 | [sdk环境](http://jingyan.baidu.com/article/f71d603757965b1ab641d12a.html)  [sdk下载](http://tools.android-studio.org/index.php/sdk/)
ant | ant -v | 

# 打包步骤
[cordova打包教程](http://www.jianshu.com/p/60e98587ae89)


```bash
#1. 安装cordova 
npm install -g cordova


# 2.检查环境
$ cordova requirement android


# 3.创建目录结构，文件夹取名为hello
$ cordova create hello

# 4.进入hello文件夹目录
$ cd hello

# 5.创建android平台
$ cordova platform add android --save

# 6.打包APP
$ cordova build
```

# 输出app
`目录 ： > hello\platforms\android\build\outputs\apk`
