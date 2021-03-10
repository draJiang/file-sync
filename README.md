# file-sync

Created By: 子龙 江
Last Edited: Mar 10, 2021 11:35 PM

## 问题

工作中在本地编辑设计源文件，同时需要将源文件备份到内部 smb 网盘中；每次源文件修改都需要更新备份或定期备份，源文件比较多时，备份工作比较麻烦。

## 方案

通过 Python 脚本自动处理备份工作。

脚本提供了 2 个功能 **配置备份任务**、**执行备份**，配置备份任务，需要输入 `本地文件地址` 、`备份地址`。执行备份时，脚本将复制本地文件到备份地址。

## 使用方法

### 搭建 Python 环境

```bash
# 安装 python3
brew install python3
# 安装 openpyxl 模块
pip3 install openpyxl
```

### 下载项目

[点击下载]([https://github.com/draJiang/file-sync/archive/main.zip](https://github.com/draJiang/file-sync/archive/main.zip))

### Windows

直接运行 `[fileSync.py](http://filesync.py/)` 

### macOS

修改 `fileSync.scpt`、`[fileSync.sh](http://filesync.sh/)` 中的路径为 `[fileSync.py](http://filesync.py/)` 的绝对路径。

直接运行 `fileSync.scpt` 或 `[fileSync.sh](http://filesync.sh/)` ；或结合 [LaunchBar]([https://www.obdev.at/products/launchbar/index.html](https://www.obdev.at/products/launchbar/index.html)) 使用。
