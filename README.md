# RiskManager 下载仓库

这里是 RiskManager 的公开下载仓库，面向使用者提供正式版 DLL、安装说明、使用教程和版本更新记录。本仓库不包含商业版源码。

RiskManager 是用于 ATAS 的 Chart Strategy，主要用途是根据固定风险金额自动计算下单手数，并辅助提交入场单、止损单和可选 RR 止盈单。

## 快速下载

| 推荐版本 | ATAS 版本 | DLL | 使用教程 | 发布说明 |
| --- | --- | --- | --- | --- |
| 4.2.2 | ATAS 8.x | [RiskManager-4.2.2.dll](正式版/8.x/RiskManager-4.2.2/RiskManager-4.2.2.dll) | [使用教程](docs/使用教程.md) | [发布说明](正式版/8.x/RiskManager-4.2.2/RELEASE_NOTES-4.2.2.md) |
| 4.2.2 | ATAS 7.x | [RiskManager-4.2.2.dll](正式版/7.x/RiskManager-4.2.2/RiskManager-4.2.2.dll) | [使用教程](docs/使用教程.md) | [发布说明](正式版/7.x/RiskManager-4.2.2/RELEASE_NOTES-4.2.2.md) |

请选择与自己 ATAS 大版本一致的 DLL。ATAS 7.x 和 ATAS 8.x 的 DLL 不能混用。

## 安装方法

1. 关闭 ATAS。
2. 下载与你 ATAS 大版本匹配的 DLL。
3. 将 DLL 复制到 ATAS Strategies 目录：

```text
%AppData%\ATAS\Strategies\
```

4. 重新启动 ATAS。
5. 打开图表，将 RiskManager 添加为 Chart Strategy。
6. 在 ATAS 底部的 Trading Strategies 列表中启用 RiskManager。

## 使用者文档

- [完整使用教程](docs/使用教程.md)
- [用户版更新日志](docs/用户版更新日志.md)
- [开源版 1.0：zhouzhen705/ATAS-RiskManager](https://github.com/zhouzhen705/ATAS-RiskManager)

## 核心功能

- 固定金额风险下单
- 图表点击选择入场价和止损价
- 自动计算下单手数
- Simple / Full 下单模式
- MKT / BID/ASK / LMT / STP 入场
- Entry / Stop Loss / Take Profit 订单流程
- RR Target 止盈计算
- Tick Value 自动识别和手动覆盖
- 风险预设按钮
- HUD 模块化显示和排序
- 中文 / 英文 HUD
- 授权码在线验证和本地授权缓存

## 正式版下载

| 版本 | ATAS | DLL | 更新日志 | 发布说明 | 说明文件 | 构建信息 |
| --- | --- | --- | --- | --- | --- | --- |
| 4.2.2 | 8.x | [DLL](正式版/8.x/RiskManager-4.2.2/RiskManager-4.2.2.dll) | [更新日志](正式版/8.x/RiskManager-4.2.2/CHANGELOG-4.2.2.md) | [发布说明](正式版/8.x/RiskManager-4.2.2/RELEASE_NOTES-4.2.2.md) | [说明文件](正式版/8.x/RiskManager-4.2.2/README-4.2.2.md) | [构建信息](正式版/8.x/RiskManager-4.2.2/BUILD_INFO-4.2.2.md) |
| 4.2.2 | 7.x | [DLL](正式版/7.x/RiskManager-4.2.2/RiskManager-4.2.2.dll) | [更新日志](正式版/7.x/RiskManager-4.2.2/CHANGELOG-4.2.2.md) | [发布说明](正式版/7.x/RiskManager-4.2.2/RELEASE_NOTES-4.2.2.md) | [说明文件](正式版/7.x/RiskManager-4.2.2/README-4.2.2.md) | [构建信息](正式版/7.x/RiskManager-4.2.2/BUILD_INFO-4.2.2.md) |
| 4.2.1 | 4.2 旧归档 | [DLL](正式版/4.2/RiskManager-4.2.1/RiskManager-4.2.1.dll) | [更新日志](正式版/4.2/RiskManager-4.2.1/CHANGELOG-4.2.1.md) | [发布说明](正式版/4.2/RiskManager-4.2.1/RELEASE_NOTES-4.2.1.md) | [说明文件](正式版/4.2/RiskManager-4.2.1/README-4.2.1.md) | [构建信息](正式版/4.2/RiskManager-4.2.1/BUILD_INFO-4.2.1.md) |
| 4.2.0 | 4.2 旧归档 | [DLL](正式版/4.2/RiskManager-4.2.0/RiskManager-4.2.0.dll) | [更新日志](正式版/4.2/RiskManager-4.2.0/CHANGELOG-4.2.0.md) | [发布说明](正式版/4.2/RiskManager-4.2.0/RELEASE_NOTES-4.2.0.md) | [说明文件](正式版/4.2/RiskManager-4.2.0/README-4.2.0.md) | [构建信息](正式版/4.2/RiskManager-4.2.0/BUILD_INFO-4.2.0.md) |
| 4.1.0 | 旧归档 | [DLL](正式版/RiskManager-4.1.0/RiskManager-4.1.0.dll) | [更新日志](正式版/RiskManager-4.1.0/CHANGELOG-4.1.0.md) | [发布说明](正式版/RiskManager-4.1.0/RELEASE_NOTES-4.1.0.md) | [说明文件](正式版/RiskManager-4.1.0/README-4.1.0.md) | [构建信息](正式版/RiskManager-4.1.0/BUILD_INFO-4.1.0.md) |

## 常见问题

HUD 没出现时，请检查 UI Style 是否为 HUD、策略是否已经添加到当前图表、ATAS 底部策略列表是否已经启用 RiskManager。

不能下单时，请检查授权码、策略启用状态、交易账户、当前品种、实时行情、Tick Value，以及 HUD 状态栏里的错误提示。

如果中文显示异常，可以在策略设置中将 HUD Language 改为 English。

## 风险提示

RiskManager 是交易执行和风险管理辅助工具，不提供交易信号、投资建议或盈利保证。实盘使用前必须先在模拟账户或回放环境中完整测试，并确认你理解每一种订单类型的行为。
