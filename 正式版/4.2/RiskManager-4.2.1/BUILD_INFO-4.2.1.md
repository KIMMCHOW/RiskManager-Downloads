# RiskManager 4.2.1 Build Info

版本：4.2.1
状态：正式版补丁
构建时间：2026-05-22

## 构建命令

```powershell
dotnet build "RiskManager 4.0\src\RiskManager.csproj" -c Release
```

## 保护命令

```powershell
.\scripts\protect-release.ps1 `
  -Version "4.2.1" `
  -SourceDll ".\RiskManager 4.0\releases\RiskManager.dll" `
  -OutputDll ".\release-archive\正式版\4.2\RiskManager-4.2.1\RiskManager-4.2.1.dll"
```

## 输出文件

- `RiskManager-4.2.1.dll`

## 变更重点

- 修复 4.2 授权机器码过于敏感导致频繁 `machine_mismatch` 的问题。
- 机器码算法升级为 v2，优先使用 Windows `MachineGuid`。
- 不再把硬盘序列号、系统盘卷序列号、MAC 地址等易变化字段混入正常机器码。

## 兼容说明

已经用 4.2 旧算法绑定过的授权，升级 4.2.1 后需要在后台重置一次 `machine_hash`，再让客户重新验证。
