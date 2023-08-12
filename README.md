# Electron-test
用Electron+Python构建一个桌面应用初步尝试，主要功能是微信运动步数修改
# -----------------------------------------------------
Python后台代码打包需要用下面的命令，否则前端开启后端服务时提示不能导入模块
    pyinstaller --onefile --hidden-import=index index.py
# -----------------------------------------------------
    
Python后台代码主程序需要加下面代码：
# 当前路径加入系统变量 ------------------------------------
import os
import sys
root_path = os.getcwd()
# print(root_path)
sys.path.append(root_path)
# -----------------------------------------------------
