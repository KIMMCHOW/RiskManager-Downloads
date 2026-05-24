# RiskManager 4.2.1 更新日志

目标版本：ATAS 8.x

## 主要更新

- 修复授权机器码过于敏感导致频繁 `machine_mismatch` 的问题。
- 机器码算法升级为 v2，优先使用 Windows `MachineGuid`。
- 不再把硬盘序列号、系统盘卷序列号、MAC 地址等易变化字段混入正常机器码。
- `MachineGuid` 读取失败时，才使用 system UUID、主板序列号、CPU ID 等较稳定字段兜底。

## 兼容说明

- 本 DLL 按当前归档规则归入 ATAS 8.x。
- 已经用 4.2 旧算法绑定过的授权，升级到 4.2.1 后需要管理员在后台重置该授权的 `machine_hash`，再让客户重新打开 ATAS 验证授权。
