# RiskManager 4.2.2 构建信息 / RiskManager 4.2.2 Build Info

## 目标 / Target

- 产品：RiskManager Pro
  Product: RiskManager Pro
- 版本：4.2.2
  Version: 4.2.2
- ATAS 目标版本：ATAS X
  ATAS target: ATAS X
- 目标框架：net10.0-windows
  Target framework: net10.0-windows

## 构建命令 / Build Command

命令：powershell.exe -ExecutionPolicy Bypass -File .\scripts\build-atas-versions.ps1 -Version 4.2.2 -Protect

Command: powershell.exe -ExecutionPolicy Bypass -File .\scripts\build-atas-versions.ps1 -Version 4.2.2 -Protect

## 输出文件 / Output

输出：release-archive\正式版\ATAS X\RiskManager-4.2.2\RiskManager-4.2.2-ATAS-X.dll

Output: release-archive\正式版\ATAS X\RiskManager-4.2.2\RiskManager-4.2.2-ATAS-X.dll

## 保护 / Protection

- 工具：Eziriz .NET Reactor
  Tool: Eziriz .NET Reactor
- 脚本：scripts\protect-release.ps1
  Script: scripts\protect-release.ps1
- 正式发布文件名不包含 protected。
  The formal release file name does not include protected.
