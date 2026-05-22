# RiskManager 4.2-A 更新日志

## 版本

RiskManager 4.2-A

## 状态

内部开发阶段版本。

## 重点

授权存储加固。

## 变更

- 授权码从本地隐藏文件 / AppData 配置迁移到 Windows 注册表。
- 注册表路径改为 `HKEY_CURRENT_USER\Software\RiskManager\License`。
- 授权码使用 Windows DPAPI 加密保存。
- 新增注册表字段：
  - `LicenseKeyEncrypted`
  - `LicenseEndpoint`
  - `LastUpdatedAt`
  - `ConfigVersion`
- 支持从 4.1 旧本地授权文件一次性迁移。
- 授权码变更后强制在线验证。
- 不再创建旧隐藏授权文件夹。
- 授权缓存改为新的安全存储方案。
- 授权日志改为新的非隐藏目录。
- 保留 Supabase 在线验证流程。
- 保留 machine_hash 绑定。
- 保留多图表复用授权码行为。

## 说明

此版本不是最终 4.2 正式版，而是 4.2 开发周期中的授权存储加固阶段版本。
