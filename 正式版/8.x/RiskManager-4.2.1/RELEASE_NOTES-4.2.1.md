# RiskManager 4.2.1 发布说明

这是适用于 ATAS 8.x 的 RiskManager 4.2.1 正式版历史归档。

本版本重点修复 4.2 机器码算法过于敏感的问题，减少正常系统变化导致的 `machine_mismatch`。正式 DLL 已通过 .NET Reactor 保护，文件名不带 `protected` 字样。

## 下载文件

```text
RiskManager-4.2.1-ATAS-8.x.dll
```

## 注意事项

- 本版本按当前归档规则归入 ATAS 8.x。
- 如果客户授权已经被 4.2 旧机器码绑定，升级 4.2.1 后需要管理员在后台重置该授权的 `machine_hash`，然后让客户重新打开 ATAS 验证授权。
