# BiliAppCacheConverter
一个将B站（哔哩哔哩，bilibili）手机app中的缓存文件合并为mp4视频和ass字幕的工具，基于Electron，flask和ffmpeg，使用nuitka和electron-builder构建

## 使用
目前仅支持Win10 / Win11

### Electron版本
- 下载release中对应的安装文件
- 像使用任何安装程序一样安装到计算机上
- 打开即用

### 原生版本
Electron构建的版本文件较大，可以选择无GUI的便携版本
- 下载release中的xxx-Windows-amd64.zip
- 解压到任意文件夹
- 运行bcc.exe
- enjoy

### 演示
[![](https://github.com/BlueCitizens/bilibili-app-cache-converter/blob/master/screenrecord.gif)](https://github.com/BlueCitizens/bilibili-app-cache-converter/blob/master/screenrecord.gif)

## 自行构建
首先打包flask，然后打包Electron

### 环境
- python 3.11 建议使用虚拟环境
- node 20.11

### build flask
使用任何python打包方式，pyinstaller和nuitka都可以正常打包。

### ffmpeg
将ffmpeg放在```/resources```目录下

### build electron
```
npm run build:win
```

## 致谢
xml弹幕文件转ass字幕文件使用了该仓库https://github.com/m13253/danmaku2ass

ffmpeg是一款强大的开源音视频软件
