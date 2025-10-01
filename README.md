这是一个win7离线安装的脚本
1、确认是win7sp1系统
2、安装NDP452-KB2901907-x86-x64-AllOS-ENU.exe
3、64位系统安装Win7AndW2K8R2-KB3191566-x64.zip/32位系统安装Win7-KB3191566-x86.zip
4、powershell  输入“$PSVersionTable.PSVersion”命令，确认powershell是5.1.xxxx.x
5、行运行：“Set-ExecutionPolicy -Scope Process -ExecutionPolicy Bypass”命令，再运行easytier.ps1脚本  或  复制easytier.ps1到powershell安装配置
注意：如有乱码报错，把脚本重新保存成“UTF-8（带 BOM）”再运行，所有语法错误都会消失。