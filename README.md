# RiskManager 下载仓库 / RiskManager Download Repository

这里是 RiskManager 的公开下载仓库，面向使用者提供正式版 DLL、安装说明、使用教程和版本更新记录。本仓库不包含商业版源码。

This is the public download repository for RiskManager. It provides release DLLs, installation instructions, the user guide, and user-facing changelogs. This repository does not contain the commercial source code.

RiskManager 是用于 ATAS 的 Chart Strategy。它根据固定风险金额自动计算下单手数，并辅助提交入场单、止损单和可选 RR 止盈单。

RiskManager is an ATAS Chart Strategy. It calculates position size from a fixed risk amount and helps submit the entry order, stop-loss order, and optional RR take-profit order.

## 快速下载 / Quick Download

请选择与自己 ATAS 版本一致的 DLL。ATAS 7.x、ATAS 8.x 和 ATAS X 的 DLL 不能混用。

Choose the DLL that matches your ATAS version. DLLs for ATAS 7.x, ATAS 8.x, and ATAS X are not interchangeable.

| 推荐版本 / Recommended | ATAS 版本 / ATAS Version | DLL | 使用教程 / User Guide | 发布说明 / Release Notes |
| --- | --- | --- | --- | --- |
| 4.6.1 | ATAS X | [RiskManager-4.6.1-ATAS-X.dll](正式版/ATAS%20X/RiskManager-4.6.1/RiskManager-4.6.1-ATAS-X.dll) | [使用教程 / User Guide](docs/使用教程.md) | [更新日志 / Changelog](docs/用户版更新日志.md) |
| 4.6.1 | ATAS 8.x | [RiskManager-4.6.1-ATAS-8.x.dll](正式版/8.x/RiskManager-4.6.1/RiskManager-4.6.1-ATAS-8.x.dll) | [使用教程 / User Guide](docs/使用教程.md) | [更新日志 / Changelog](docs/用户版更新日志.md) |
| 4.6.1 | ATAS 7.x | [RiskManager-4.6.1-ATAS-7.x.dll](正式版/7.x/RiskManager-4.6.1/RiskManager-4.6.1-ATAS-7.x.dll) | [使用教程 / User Guide](docs/使用教程.md) | [更新日志 / Changelog](docs/用户版更新日志.md) |

## 安装方法 / Installation

1. 关闭 ATAS。
   Close ATAS.
2. 下载与你 ATAS 大版本匹配的 DLL。
   Download the DLL that matches your ATAS major version.
3. 将 DLL 复制到 ATAS Strategies 目录。
   Copy the DLL into the ATAS Strategies folder.

```text
%AppData%\ATAS\Strategies\
```

4. 重新启动 ATAS。
   Restart ATAS.
5. 打开图表，将 RiskManager 添加为 Chart Strategy。
   Open a chart and add RiskManager as a Chart Strategy.
6. 在 ATAS 底部的 Trading Strategies 列表中启用 RiskManager。
   Enable RiskManager from the Trading Strategies list at the bottom of ATAS.

## 使用者文档 / User Documents

- [完整使用教程 / Full User Guide](docs/使用教程.md)
- [用户版更新日志 / User Changelog](docs/用户版更新日志.md)
- [开源版 1.0 / Open-source 1.0: KIMMCHOW/ATAS-RiskManager](https://github.com/KIMMCHOW/ATAS-RiskManager)

## 核心功能 / Core Features

- 固定金额风险下单。
  Fixed-risk amount order entry.
- 图表点击选择入场价和止损价。
  Click on the chart to choose entry and stop prices.
- 自动计算下单手数。
  Automatic position-size calculation.
- Simple / Full 下单模式。
  Simple / Full order modes.
- MKT / BID/ASK / LMT / STP 入场。
  MKT / BID/ASK / LMT / STP entry types.
- Entry / Stop Loss / Take Profit 订单流程。
  Entry / Stop Loss / Take Profit order workflow.
- RR Target 止盈计算。
  RR Target take-profit calculation.
- Tick Value 自动识别和手动覆盖。
  Automatic Tick Value detection and manual override.
- 风险预设按钮。
  Risk preset buttons.
- HUD 模块化显示和排序。
  Modular HUD display and ordering.
- HUD 与设置界面自动跟随 ATAS 界面语言（支持英文、简体中文、德语、西班牙语、法语、印地语、意大利语、日语、韩语、葡萄牙语、俄语）。
  HUD and settings automatically follow the ATAS interface language (English, Simplified Chinese, German, Spanish, French, Hindi, Italian, Japanese, Korean, Portuguese, and Russian).
- 授权码在线验证和本地授权缓存。
  Online license validation and local license cache.

## 正式版下载 / Formal Release Downloads

| 版本 / Version | ATAS | DLL | 更新日志 / Changelog | 发布说明 / Release Notes | 说明文件 / README | 构建信息 / Build Info |
| --- | --- | --- | --- | --- | --- | --- |
| 4.6.1 | ATAS X | [DLL](正式版/ATAS%20X/RiskManager-4.6.1/RiskManager-4.6.1-ATAS-X.dll) | [更新日志 / Changelog](docs/用户版更新日志.md) | — | — | — |
| 4.6.1 | 8.x | [DLL](正式版/8.x/RiskManager-4.6.1/RiskManager-4.6.1-ATAS-8.x.dll) | [更新日志 / Changelog](docs/用户版更新日志.md) | — | — | — |
| 4.6.1 | 7.x | [DLL](正式版/7.x/RiskManager-4.6.1/RiskManager-4.6.1-ATAS-7.x.dll) | [更新日志 / Changelog](docs/用户版更新日志.md) | — | — | — |
| 4.6.0 | ATAS X | [DLL](正式版/ATAS%20X/RiskManager-4.6.0/RiskManager-4.6.0-ATAS-X.dll) | [更新日志 / Changelog](docs/用户版更新日志.md) | — | — | — |
| 4.6.0 | 8.x | [DLL](正式版/8.x/RiskManager-4.6.0/RiskManager-4.6.0-ATAS-8.x.dll) | [更新日志 / Changelog](docs/用户版更新日志.md) | — | — | — |
| 4.6.0 | 7.x | [DLL](正式版/7.x/RiskManager-4.6.0/RiskManager-4.6.0-ATAS-7.x.dll) | [更新日志 / Changelog](docs/用户版更新日志.md) | — | — | — |
| 4.5.0 | ATAS X | [DLL](正式版/ATAS%20X/RiskManager-4.5.0/RiskManager-4.5.0-ATAS-X.dll) | [更新日志 / Changelog](docs/用户版更新日志.md) | — | — | — |
| 4.5.0 | 8.x | [DLL](正式版/8.x/RiskManager-4.5.0/RiskManager-4.5.0-ATAS-8.x.dll) | [更新日志 / Changelog](docs/用户版更新日志.md) | — | — | — |
| 4.5.0 | 7.x | [DLL](正式版/7.x/RiskManager-4.5.0/RiskManager-4.5.0-ATAS-7.x.dll) | [更新日志 / Changelog](docs/用户版更新日志.md) | — | — | — |
| 4.3.0 | ATAS X | [DLL](正式版/ATAS%20X/RiskManager-4.3.0/RiskManager-4.3.0-ATAS-X.dll) | — | — | — | — |
| 4.3.0 | 8.x | [DLL](正式版/8.x/RiskManager-4.3.0/RiskManager-4.3.0-ATAS-8.x.dll) | — | — | — | — |
| 4.3.0 | 7.x | [DLL](正式版/7.x/RiskManager-4.3.0/RiskManager-4.3.0-ATAS-7.x.dll) | — | — | — | — |
| 4.2.6 | ATAS X | [DLL](正式版/ATAS%20X/RiskManager-4.2.6/RiskManager-4.2.6-ATAS-X.dll) | [更新日志 / Changelog](正式版/ATAS%20X/RiskManager-4.2.6/CHANGELOG-4.2.6.md) | [发布说明 / Release Notes](正式版/ATAS%20X/RiskManager-4.2.6/RELEASE_NOTES-4.2.6.md) | [说明文件 / README](正式版/ATAS%20X/RiskManager-4.2.6/README-4.2.6.md) | [构建信息 / Build Info](正式版/ATAS%20X/RiskManager-4.2.6/BUILD_INFO-4.2.6.md) |
| 4.2.6 | 8.x | [DLL](正式版/8.x/RiskManager-4.2.6/RiskManager-4.2.6-ATAS-8.x.dll) | [更新日志 / Changelog](正式版/8.x/RiskManager-4.2.6/CHANGELOG-4.2.6.md) | [发布说明 / Release Notes](正式版/8.x/RiskManager-4.2.6/RELEASE_NOTES-4.2.6.md) | [说明文件 / README](正式版/8.x/RiskManager-4.2.6/README-4.2.6.md) | [构建信息 / Build Info](正式版/8.x/RiskManager-4.2.6/BUILD_INFO-4.2.6.md) |
| 4.2.6 | 7.x | [DLL](正式版/7.x/RiskManager-4.2.6/RiskManager-4.2.6-ATAS-7.x.dll) | [更新日志 / Changelog](正式版/7.x/RiskManager-4.2.6/CHANGELOG-4.2.6.md) | [发布说明 / Release Notes](正式版/7.x/RiskManager-4.2.6/RELEASE_NOTES-4.2.6.md) | [说明文件 / README](正式版/7.x/RiskManager-4.2.6/README-4.2.6.md) | [构建信息 / Build Info](正式版/7.x/RiskManager-4.2.6/BUILD_INFO-4.2.6.md) |
| 4.2.5 | ATAS X | [DLL](正式版/ATAS%20X/RiskManager-4.2.5/RiskManager-4.2.5-ATAS-X.dll) | [更新日志 / Changelog](正式版/ATAS%20X/RiskManager-4.2.5/CHANGELOG-4.2.5.md) | [发布说明 / Release Notes](正式版/ATAS%20X/RiskManager-4.2.5/RELEASE_NOTES-4.2.5.md) | [说明文件 / README](正式版/ATAS%20X/RiskManager-4.2.5/README-4.2.5.md) | [构建信息 / Build Info](正式版/ATAS%20X/RiskManager-4.2.5/BUILD_INFO-4.2.5.md) |
| 4.2.5 | 8.x | [DLL](正式版/8.x/RiskManager-4.2.5/RiskManager-4.2.5-ATAS-8.x.dll) | [更新日志 / Changelog](正式版/8.x/RiskManager-4.2.5/CHANGELOG-4.2.5.md) | [发布说明 / Release Notes](正式版/8.x/RiskManager-4.2.5/RELEASE_NOTES-4.2.5.md) | [说明文件 / README](正式版/8.x/RiskManager-4.2.5/README-4.2.5.md) | [构建信息 / Build Info](正式版/8.x/RiskManager-4.2.5/BUILD_INFO-4.2.5.md) |
| 4.2.5 | 7.x | [DLL](正式版/7.x/RiskManager-4.2.5/RiskManager-4.2.5-ATAS-7.x.dll) | [更新日志 / Changelog](正式版/7.x/RiskManager-4.2.5/CHANGELOG-4.2.5.md) | [发布说明 / Release Notes](正式版/7.x/RiskManager-4.2.5/RELEASE_NOTES-4.2.5.md) | [说明文件 / README](正式版/7.x/RiskManager-4.2.5/README-4.2.5.md) | [构建信息 / Build Info](正式版/7.x/RiskManager-4.2.5/BUILD_INFO-4.2.5.md) |
| 4.2.4 | ATAS X | [DLL](正式版/ATAS%20X/RiskManager-4.2.4/RiskManager-4.2.4-ATAS-X.dll) | [更新日志 / Changelog](正式版/ATAS%20X/RiskManager-4.2.4/CHANGELOG-4.2.4.md) | [发布说明 / Release Notes](正式版/ATAS%20X/RiskManager-4.2.4/RELEASE_NOTES-4.2.4.md) | [说明文件 / README](正式版/ATAS%20X/RiskManager-4.2.4/README-4.2.4.md) | [构建信息 / Build Info](正式版/ATAS%20X/RiskManager-4.2.4/BUILD_INFO-4.2.4.md) |
| 4.2.4 | 8.x | [DLL](正式版/8.x/RiskManager-4.2.4/RiskManager-4.2.4-ATAS-8.x.dll) | [更新日志 / Changelog](正式版/8.x/RiskManager-4.2.4/CHANGELOG-4.2.4.md) | [发布说明 / Release Notes](正式版/8.x/RiskManager-4.2.4/RELEASE_NOTES-4.2.4.md) | [说明文件 / README](正式版/8.x/RiskManager-4.2.4/README-4.2.4.md) | [构建信息 / Build Info](正式版/8.x/RiskManager-4.2.4/BUILD_INFO-4.2.4.md) |
| 4.2.4 | 7.x | [DLL](正式版/7.x/RiskManager-4.2.4/RiskManager-4.2.4-ATAS-7.x.dll) | [更新日志 / Changelog](正式版/7.x/RiskManager-4.2.4/CHANGELOG-4.2.4.md) | [发布说明 / Release Notes](正式版/7.x/RiskManager-4.2.4/RELEASE_NOTES-4.2.4.md) | [说明文件 / README](正式版/7.x/RiskManager-4.2.4/README-4.2.4.md) | [构建信息 / Build Info](正式版/7.x/RiskManager-4.2.4/BUILD_INFO-4.2.4.md) |
| 4.2.2 | ATAS X | [DLL](正式版/ATAS%20X/RiskManager-4.2.2/RiskManager-4.2.2-ATAS-X.dll) | [更新日志 / Changelog](正式版/ATAS%20X/RiskManager-4.2.2/CHANGELOG-4.2.2.md) | [发布说明 / Release Notes](正式版/ATAS%20X/RiskManager-4.2.2/RELEASE_NOTES-4.2.2.md) | [说明文件 / README](正式版/ATAS%20X/RiskManager-4.2.2/README-4.2.2.md) | [构建信息 / Build Info](正式版/ATAS%20X/RiskManager-4.2.2/BUILD_INFO-4.2.2.md) |
| 4.2.2 | 8.x | [DLL](正式版/8.x/RiskManager-4.2.2/RiskManager-4.2.2-ATAS-8.x.dll) | [更新日志 / Changelog](正式版/8.x/RiskManager-4.2.2/CHANGELOG-4.2.2.md) | [发布说明 / Release Notes](正式版/8.x/RiskManager-4.2.2/RELEASE_NOTES-4.2.2.md) | [说明文件 / README](正式版/8.x/RiskManager-4.2.2/README-4.2.2.md) | [构建信息 / Build Info](正式版/8.x/RiskManager-4.2.2/BUILD_INFO-4.2.2.md) |
| 4.2.2 | 7.x | [DLL](正式版/7.x/RiskManager-4.2.2/RiskManager-4.2.2-ATAS-7.x.dll) | [更新日志 / Changelog](正式版/7.x/RiskManager-4.2.2/CHANGELOG-4.2.2.md) | [发布说明 / Release Notes](正式版/7.x/RiskManager-4.2.2/RELEASE_NOTES-4.2.2.md) | [说明文件 / README](正式版/7.x/RiskManager-4.2.2/README-4.2.2.md) | [构建信息 / Build Info](正式版/7.x/RiskManager-4.2.2/BUILD_INFO-4.2.2.md) |
| 4.2.1 | 8.x | [DLL](正式版/8.x/RiskManager-4.2.1/RiskManager-4.2.1-ATAS-8.x.dll) | [更新日志 / Changelog](正式版/8.x/RiskManager-4.2.1/CHANGELOG-4.2.1.md) | [发布说明 / Release Notes](正式版/8.x/RiskManager-4.2.1/RELEASE_NOTES-4.2.1.md) | [说明文件 / README](正式版/8.x/RiskManager-4.2.1/README-4.2.1.md) | [构建信息 / Build Info](正式版/8.x/RiskManager-4.2.1/BUILD_INFO-4.2.1.md) |
| 4.2.0 | 8.x | [DLL](正式版/8.x/RiskManager-4.2.0/RiskManager-4.2.0-ATAS-8.x.dll) | [更新日志 / Changelog](正式版/8.x/RiskManager-4.2.0/CHANGELOG-4.2.0.md) | [发布说明 / Release Notes](正式版/8.x/RiskManager-4.2.0/RELEASE_NOTES-4.2.0.md) | [说明文件 / README](正式版/8.x/RiskManager-4.2.0/README-4.2.0.md) | [构建信息 / Build Info](正式版/8.x/RiskManager-4.2.0/BUILD_INFO-4.2.0.md) |

## 常见问题 / FAQ

HUD 没出现时，请检查 UI Style 是否为 HUD、策略是否已经添加到当前图表、ATAS 底部策略列表是否已经启用 RiskManager。

If the HUD does not appear, check whether UI Style is set to HUD, whether the strategy has been added to the current chart, and whether RiskManager is enabled in the ATAS bottom Trading Strategies list.

不能下单时，请检查授权码、策略启用状态、交易账户、当前品种、实时行情、Tick Value，以及 HUD 状态栏里的错误提示。

If orders cannot be submitted, check the License Key, strategy activation state, trading account, current instrument, live market data, Tick Value, and the error message in the HUD status line.

RiskManager 的界面文字跟随 ATAS 界面语言显示。如需切换语言，请在 ATAS 主窗口右上角点击个人资料图标并选择 Language，然后重启相关窗口。

RiskManager text follows the ATAS interface language. To switch it, click the Profile icon in the upper-right corner of the main ATAS window, select Language, then restart the affected windows.

## 风险提示 / Risk Notice

RiskManager 是交易执行和风险管理辅助工具，不提供交易信号、投资建议或盈利保证。实盘使用前必须先在模拟账户或回放环境中完整测试，并确认你理解每一种订单类型的行为。

RiskManager is a trade execution and risk-management assistant. It does not provide trading signals, investment advice, or any profit guarantee. Before live trading, test it thoroughly in simulation or replay and make sure you understand how each order type behaves.
