# RiskManager 4.2.5 发布说明 / RiskManager 4.2.5 Release Notes

## 修复 / Fixed

- 修复 BID / ASK 报价与当前成交价相同时可能取消下单设置的问题。
  Fixed an edge case where BID / ASK order setup could be canceled when the live quote matched the current traded price.
- 当实时买卖价不可用时，流程会安全停止并显示明确提示。
  When the live bid or ask is unavailable, the setup stops safely with a clear message.

## 优化 / Improved

- 提高等待设置止损时的入场价跟踪响应。
  Improved entry-price tracking responsiveness while waiting for stop placement.
- 保持现有 LMT / STP 价格关系和止损方向校验不变。
  Preserved the existing LMT / STP price-relationship and stop-direction validation.
