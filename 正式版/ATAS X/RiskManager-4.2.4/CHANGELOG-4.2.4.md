# RiskManager 4.2.4 变更记录 / RiskManager 4.2.4 Changelog

- 发布 RiskManager 4.2.4 ATAS X 正式保护版 DLL。
  Published the formal protected RiskManager 4.2.4 DLL for ATAS X.
- Market / Bid / Ask 入场价同步节流从 50ms 调整为 20ms，提升等待设置 SL 时的跟价响应。
  Market / Bid / Ask entry-price sync throttling changed from 50ms to 20ms for faster tracking while waiting for SL placement.
- ENTRY / SL / TP 参考线改为只在最终绘制层渲染，并在实时入场价变化时请求图表重绘，减少旧价线残留。
  ENTRY / SL / TP reference lines now render only on the final drawing layer and request chart redraws when live entry price changes, reducing stale level remnants.
- 当 entry / stop / market 价格关系无效时，当前下单流程会直接取消并清空价线，用户需要重新点击 HUD 下单按钮。
  When the entry / stop / market price relationship is invalid, the current order setup is canceled and level lines are cleared; users must click a HUD order button again.
