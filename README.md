# BBDown-Extension-tools
**一个可选功能完全没有的垃圾的BBDownGUI实现(可通过BBDown.config实现配置)，但有输入校验与文件自动整理功能，需要自行准备BBDown.exe**

- **请在程序根目录添加icon.ico文件，否则会报错**   
- 请自行修改BD.config文件：  
- **第一行不要改**   
- 第二行为BBDown.exe的路径(**可为相对路径或绝对路径**)   
- 第三行为下载的目标目录，请自行更改（**默认为C:\BilibiliDownloadFile**)  
- 第四行为7 zip的目录(**不支持WinRAR**)(**可以在这一行的等号后写False或等号后为空来不压缩，但等号前面要留下**)   

以下为一个BD.config的实例:   
  ```
  [DefaultDirectory]
  BBDownDirectory=BBDown_win-x64\BBDown.exe
  DownloadTheDefaultDirectory=D:\BilibiliDownloadFile\
  DirectoryOf7z=C:\Program Files\7-Zip\7z.exe
  ```
**不再提供二进制文件，请自行编译**  
**需要使用的模块如下：**
- ctypes
- tkinter
- threading
- json
- re
- os
- subprocess
- requests
- configparser
- pywin32

# 使用方法
1. 下载[BBDown](https://github.com/nilaoda/BBDown)(**最好为最新action**)
2. 在电脑上安装好python的最新版本
3. 下载本项目源代码
4. 把BBdown拷贝入源代码根目录
5. 在根目录添加BBDown.config文件
6. 修改第二行BBDown程序的目录
7. 修改第三行下载目标路径(**如果设置了BBDown的工作目录则要与工作目录相同，否则就在BBDown.exe的所在路径**)
8. 在根目录添加icon.ico文件，内容随意
9. 双击GUI.py即可开始运行

## 感谢名单：
https://github.com/nilaoda/BBDown  
https://github.com/Jianningyuan/bilibili-API-collect
## 特别鸣谢：
由Microsoft提供的独立源代码编辑器  
**VSCode**  

![VSCode](https://user-images.githubusercontent.com/102419562/184617892-8f1d0fed-34b0-44cc-b7c3-cab19a5d23f6.png)

**An optional function completely does not have the garbage BBDownGUI implementation (can be configured through BBDown.config), but there is input verification and file automatic sorting function, you need to prepare your own BBDown.exe**

- **Please add the icon .ico file in the root directory of the program, otherwise an error will be reported**
- Please modify the BD.config file yourself:
- **Do not change the first line**
- The path of the second line BBDown.exe (**can be relative or absolute**)
- The third line downloads the target directory, please change it yourself (default is **C:BilibiliDownloadFile**)
- Fourth line 7 zip directory (WinRAR is not supported) (**False can be written after the equal sign of this line or blank after the equal sign to not compress, but leave the equal sign in front of it**)  

The following is an example of BD.config:  
  ```
  [DefaultDirectory]
  BBDownDirectory=BBDown_win-x64\BBDown.exe
  DownloadTheDefaultDirectory=D:\BilibiliDownloadFile\
  DirectoryOf7z=C:\Program Files\7-Zip\7z.exe
  ```
**Binaries are no longer provided, please compile yourself**  
**The following modules need to be used:**
- ctypes
- tkinter
- threading
- json
- re
- os
- subprocess
- requests
- configparser
- pywin32
