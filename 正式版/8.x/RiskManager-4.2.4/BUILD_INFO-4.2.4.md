# RiskManager 4.2.4 构建信息 / RiskManager 4.2.4 Build Info

## 构建 / Build

- 产品：RiskManager
  Product: RiskManager
- 版本：4.2.4
  Version: 4.2.4
- ATAS 目标：8.x
  ATAS target: 8.x
- 目标框架：`net10.0-windows`
  Target framework: `net10.0-windows`
- DLL：`RiskManager-4.2.4-ATAS-8.x.dll`
  DLL: `RiskManager-4.2.4-ATAS-8.x.dll`

## 命令 / Command

命令：`powershell.exe -ExecutionPolicy Bypass -File .\scripts\build-atas-versions.ps1 -Version 4.2.4 -Protect`

Command: `powershell.exe -ExecutionPolicy Bypass -File .\scripts\build-atas-versions.ps1 -Version 4.2.4 -Protect`

## 保护 / Protection

- 正式 DLL 已通过 .NET Reactor 保护。
  The formal DLL is protected with .NET Reactor.
- 保护基线与 Options Level Pro 托管 DLL 的 Baseline profile 保持一致，并保留 ATAS 需要的 public 反射表面。
  The protection baseline matches the Options Level Pro managed-DLL Baseline profile and preserves the public reflection surface required by ATAS.
