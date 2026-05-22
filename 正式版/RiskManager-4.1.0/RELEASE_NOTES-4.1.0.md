# RiskManager 4.1.0 发布说明

RiskManager 4.1.0 是 RiskManager 的正式发布版本。

它是用于 ATAS 的 Chart Strategy，主要用于固定风险金额下单和图表化订单执行。用户可以输入单笔交易愿意承担的风险金额，在图表上选择入场价和止损价，RiskManager 会自动计算下单数量。

此版本包含 Simple 和 Full 两种下单模式，支持 MKT / LMT / STP 入场，支持 RR Target 计算、SL / TP / OCO 处理、Tick Value 自动识别和手动设置、中文 / 英文 HUD，以及基于 Supabase 的在线授权验证。

## 重要说明

- RiskManager 是交易执行和风险管理辅助工具。
- RiskManager 不提供交易信号。
- RiskManager 不提供投资建议。
- RiskManager 不保证盈利。
- 实盘使用前必须先在模拟盘或回放环境中完整测试。
- 授权存储和 DLL 保护会在 4.2 版本继续增强。
