# Win7 离线安装脚本说明

## 安装步骤

1. **确认系统版本**  
   确认当前为 Windows 7 SP1 系统。

2. **安装 .NET Framework 4.5.2**  
   运行 `NDP452-KB2901907-x86-x64-AllOS-ENU.exe` 安装程序。

3. **安装 KB3191566 补丁**  
   - 64 位系统：安装 `Win7AndW2K8R2-KB3191566-x64.zip`  
   - 32 位系统：安装 `Win7-KB3191566-x86.zip`

4. **确认 PowerShell 版本**  
   在 PowerShell 中输入以下命令，确认版本为 5.1.xxxx.x：  
   ```powershell
   $PSVersionTable.PSVersion
   ```

5. **运行安装脚本**  
   在 PowerShell 中依次执行以下命令：  
   ```powershell
   Set-ExecutionPolicy -Scope Process -ExecutionPolicy Bypass
   .\easytier.ps1
   ```
   或将 `easytier.ps1` 复制到 PowerShell 安装目录后运行。

> **注意**  
> 如遇乱码报错，请将脚本重新保存为 “UTF-8（带 BOM）” 格式后再运行，所有语法错误都会消失。
## 离线依赖包
- [.NET Framework 4.5.2](https://github.com/renlu99/EasyTier-Win7-Offline/releases/download/V1/NDP452-KB2901907-x86-x64-AllOS-ENU.exe)
- [Windows 7 32位更新补丁 KB3191566](https://github.com/renlu99/EasyTier-Win7-Offline/releases/download/V1/Win7-KB3191566-x86.zip)
- [Windows 7 64位更新补丁 KB3191566](https://github.com/renlu99/EasyTier-Win7-Offline/releases/download/V1/Win7AndW2K8R2-KB3191566-x64.zip)
- [easytier.ps1](https://github.com/renlu99/EasyTier-Win7-Offline/releases/download/V1/easytier.ps1)
- [easytier-windows-x86_64-v2.4.5.zip](https://github.com/renlu99/EasyTier-Win7-Offline/releases/download/V1/easytier-windows-x86_64-v2.4.5.zip)