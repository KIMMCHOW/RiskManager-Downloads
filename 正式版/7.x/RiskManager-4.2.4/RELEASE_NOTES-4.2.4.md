# RiskManager 4.2.4 发布说明 / RiskManager 4.2.4 Release Notes

## 优化 / Improved

- Market / Bid / Ask 入场参考线在等待设置 SL 时更快跟随最新价格。
  Market / Bid / Ask entry reference lines track the latest price faster while waiting for SL placement.
- 优化参考线刷新方式，减少首次点击和实时跟价过程中旧价线残留。
  Improved reference-line refresh behavior to reduce stale lines during first click and live price tracking.
- 无效价格关系现在会取消本次下单流程并清空价线，避免用户误以为仍在等待下单。
  Invalid price relationships now cancel the current order setup and clear level lines, preventing users from thinking the setup is still pending.
