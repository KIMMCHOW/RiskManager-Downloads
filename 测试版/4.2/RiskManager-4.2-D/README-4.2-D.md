# RiskManager 4.2-D 归档

此目录保存 RiskManager 4.2-D 阶段版本的 DLL、protected DLL 和发布文档。

## 文件

- RiskManager-4.2-D.dll
- RiskManager-4.2-D.protected.dll
- CHANGELOG-4.2-D.md
- RELEASE_NOTES-4.2-D.md
- BUILD_INFO-4.2-D.md
- README-4.2-D.md

## 范围

此阶段版本重点是：

- 风险预设按钮
- 风险预设启用 / 禁用设置
- 风险预设模块默认排在 HUD 第一个
- HUD 模块默认排序使用 1-7
- HUD Modules 设置组中加入 Show Risk Preset Module
- 订单按钮显示开关
- Cancel Button Mode
- Cancel 二次确认
- 当前账户、当前品种订单撤销和仓位关闭
- Cancel 订单和仓位处理改为非阻塞异步流程，避免点击后卡死

## 保护后 DLL 状态

`RiskManager-4.2-D.protected.dll` 已使用根目录 `scripts\protect-release.ps1` 生成。

使用的 .NET Reactor Console 路径：

```text
C:\Program Files (x86)\Eziriz\.NET Reactor\dotNET_Reactor.Console.exe
```

## 风险提示

这是内部开发阶段版本，不是最终公开发布的 RiskManager 4.2 正式版。

如果 Cancel Scope 选择当前品种订单和仓位，Cancel 会在二次确认后撤销当前账户、当前图表品种的未成交订单，并调用 ATAS 官方持仓关闭流程处理当前品种仓位。实盘前必须先在模拟环境验证。
