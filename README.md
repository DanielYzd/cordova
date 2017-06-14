# cordova
![image](https://user-images.githubusercontent.com/18028533/27120577-b9a728d0-5116-11e7-94a2-8cd55266ba04.png)

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


# （可选步骤）2.检查环境
$ cordova requirement android


# 3.创建目录结构，文件夹取名为hello
$ cordova create hello


# 4.进入hello文件夹目录
$ cd hello


# 5.创建android平台
$ cordova platform add android --save


# (可选步骤)6.安装plugin cordova-hot-code-push-plugin：
cordova plugin add cordova-hot-code-push-plugin


# (可选步骤)7.安装plugin com.badrit.MacAddress
$ cordova plugin add com.badrit.MacAddress


# （可选步骤）8.全局安装 cordova-hot-code-push-cl:
$ npm install -g cordova-hot-code-push-cli

```


# 打包APP(注：目录中不能有汉字，不然报错)
```bash
$ cordova build
```


# 输出app
`目录 ： > hello\platforms\android\build\outputs\apk`
