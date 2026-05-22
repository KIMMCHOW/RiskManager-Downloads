# RiskManager 4.2.0 发布说明

RiskManager 4.2.0 是 RiskManager 的正式发布版本。

本版本重点完成授权加固和 HUD 体验增强，同时加入风险预设按钮、订单按钮显示控制、Cancel 二次确认和当前品种订单 / 仓位处理能力。正式 DLL 已经过 .NET Reactor 保护，文件名为 `RiskManager-4.2.0.dll`。

## 授权

- 授权码保存位置迁移到 `HKEY_CURRENT_USER\Software\RiskManager\License`。
- 授权码使用 Windows DPAPI 加密保存。
- 支持从 4.1 旧本地授权文件迁移。
- 授权码变更后会强制在线验证。
- 不再创建旧隐藏授权文件夹。

## HUD

- HUD 支持模块化显示。
- 支持模块开关、模块内小项开关和数字排序。
- 风险预设模块默认显示在 HUD 最上方。
- 下单模式默认完整。

## 风险预设和订单按钮

- 新增 200 / 500 / 1000 / 2000 风险预设按钮。
- 每个风险预设按钮可单独启用 / 禁用。
- MKT / BID/ASK / LMT / STP / Cancel 按钮可单独控制显示。

## Cancel 行为

Cancel 默认只清空当前 RiskManager 操作流程。

如果启用订单和仓位处理模式，并通过二次确认，RiskManager 会撤销当前账户、当前图表品种下的可撤订单，并调用 ATAS 官方持仓关闭流程处理当前图表品种仓位。

## 使用教程

完整中文使用教程位于项目根目录：

```text
使用教程.md
```

## 风险提示

- RiskManager 是交易执行和风险管理工具，不提供交易信号。
- RiskManager 不提供投资建议，也不保证盈利。
- Cancel 订单和仓位处理属于真实交易操作。
- 使用 Cancel 订单和仓位处理前，必须确认当前账户和图表品种正确。
- 实盘使用前必须先在模拟环境完整测试。
