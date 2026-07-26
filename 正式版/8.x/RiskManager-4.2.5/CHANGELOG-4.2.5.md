# RiskManager 4.2.5 变更记录 / RiskManager 4.2.5 Changelog

- 发布 RiskManager 4.2.5 ATAS 8.x 正式保护版 DLL。
  Published the formal protected RiskManager 4.2.5 DLL for ATAS 8.x.
- 修复 BID / ASK 报价与当前成交价相同时可能取消下单设置的问题。
  Fixed an edge case where BID / ASK order setup could be canceled when the live quote matched the current traded price.
- 提高等待设置止损时的实时入场价跟踪频率。
  Increased live entry-price tracking frequency while waiting for stop placement.
- 当实时买卖价不可用时安全停止流程，并显示更明确的状态提示。
  Stops the setup safely with a clearer status message when the live bid or ask is unavailable.
- 保持手动画 LMT / STP 入场和止损方向规则不变。
  Preserves the existing chart-selected LMT / STP and stop-direction rules.
