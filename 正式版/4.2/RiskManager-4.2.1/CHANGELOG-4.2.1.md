# RiskManager 4.2.1 Changelog

RiskManager 4.2.1 是 4.2 正式版的授权稳定性补丁版本。

## Fixed

- 修复授权机器码频繁变化导致 `machine_mismatch` 的问题。
- 机器码生成逻辑改为优先使用 Windows `MachineGuid`。
- 移除正常机器码中的硬盘序列号、系统盘卷序列号、MAC 地址等易变化字段，降低系统环境变化导致授权失效的概率。

## Changed

- 版本号更新为 `4.2.1`。
- 机器码算法升级为 v2。

## Upgrade Notes

- 已经用 4.2 旧算法绑定过的授权，升级到 4.2.1 后需要管理员在后台重置该授权的 `machine_hash`，再让客户重新打开 ATAS 验证授权。
- 本版本不改变交易功能。
- 本版本不改变 4.3 Web 后台功能。
- 本版本不删除或迁移旧授权数据。
