# pyqt_orc
使用pyqt5做的一个简单图形的orc识别

**找到最新版了 -_-**

### 使用
修改 config.ini 中的配置为自己的 在百度申请的id key 等 就可以使用
快捷键 F4 可以直接截图识别

### python3+ 运行

```bash
git clone https://github.com/libaibuaidufu/pyqt_orc.git
cd pyqt_orc
pip install -r requirements.txt
python main.py
```

### pyinstaller 打包命令

```bash
windows（已测试-单文件无法保存配置）：
pyinstaller -F -w main.py -i image/logo.ico --add-data config/config.ini;config --add-data image/logo.ico;image
linux（未测试）:
pyinstaller -F -w main.py -i image/logo.ico --add-data config/config.ini:config --add-data image/logo.ico:image
windows（已测试-文件夹可以保存配置-类似于安装版）：
pyinstaller -D -w main.py -i image/logo.ico --add-data config/config.ini;config --add-data image/logo.ico;image
```

###### 2020-1-12 更新

1. 已经更新为省去图片保存 直接转byte
2. 同时修改 鼠标样式 更加显著的 截图标识
3. 发现问题 应用 必须要自己打包使用，因为配置保存只能此次打开有用。
4. 3的问题有缘再解决了



### 问题

图片会保存本地 再删除 耽误时间 可以更好的直接传送字节过去 省去这一步

### 预览
![image](https://github.com/libaibuaidufu/pyqt_orc/blob/master/last.png)