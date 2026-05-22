# RiskManager 4.2.0 构建信息

## 版本

RiskManager 4.2.0

## 构建配置

Release

## 项目

src/RiskManager.csproj

## 未保护输出 DLL

```text
RiskManager 4.0\releases\RiskManager.dll
```

## 正式版 DLL

```text
release-archive\正式版\4.2\RiskManager-4.2.0\RiskManager-4.2.0.dll
```

## 构建命令

```powershell
dotnet build src\RiskManager.csproj -c Release
```

## 保护命令

```powershell
.\scripts\protect-release.ps1 -Version "4.2.0" -SourceDll ".\RiskManager 4.0\releases\RiskManager.dll" -OutputDll ".\release-archive\正式版\4.2\RiskManager-4.2.0\RiskManager-4.2.0.dll"
```

## Git Commit

Git commit not available.

## 构建时间

2026-05-21 19:54:04 +08:00

## Protection

Protection tool:
Eziriz .NET Reactor 7.3.0.0

Protection script:
scripts/protect-release.ps1

Protection status:
Generated

正式版 DLL 已保护，但文件名不带 `protected` 字样。

Protection parameters:

```text
-suppressildasm 1
-control_flow 1
-flow_level 3
-obfuscation 1
-obfuscate_public_types 0
-virtualization 0
-internalization 0
-antitamp 0
-nodialog
-licensed
```
