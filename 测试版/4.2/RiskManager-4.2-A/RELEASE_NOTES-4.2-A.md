# RiskManager 4.2-A 发布说明

RiskManager 4.2-A 是 RiskManager 4.2 开发周期中的内部阶段版本。

此版本重点是授权存储加固。授权码不再写入本地隐藏文件 / AppData 配置，而是写入当前用户的 Windows 注册表，并使用 Windows DPAPI 加密。

## 重点说明

- 这不是最终 RiskManager 4.2 正式版。
- 此版本用于内部测试。
- 授权码存储位置为 `HKEY_CURRENT_USER\Software\RiskManager\License`。
- 授权码在注册表中以加密形式保存。
- 4.1 旧授权文件只用于一次性迁移。
- 后续阶段继续完善 HUD 模块化、风险预设按钮和 DLL 保护发布流程。
