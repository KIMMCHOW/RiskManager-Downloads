# RiskManager 4.2.1

RiskManager 4.2.1 是 4.2 正式版的授权稳定性补丁，推荐所有 4.2 正式版用户升级。

## 下载

- [RiskManager-4.2.1.dll](RiskManager-4.2.1.dll)

## 版本说明

- [CHANGELOG-4.2.1.md](CHANGELOG-4.2.1.md)
- [RELEASE_NOTES-4.2.1.md](RELEASE_NOTES-4.2.1.md)
- [BUILD_INFO-4.2.1.md](BUILD_INFO-4.2.1.md)

## 主要修复

- 修复授权机器码频繁变化导致 `machine_mismatch` 的问题。
- 机器码生成逻辑改为优先使用 Windows `MachineGuid`。
- 不再把硬盘序列号、系统盘卷序列号、MAC 地址等易变化字段混入正常机器码。

## 升级注意

如果客户授权已经被 4.2 旧机器码绑定，升级 4.2.1 后需要管理员在后台重置该授权的 `machine_hash`，然后让客户重新打开 ATAS 验证授权。
