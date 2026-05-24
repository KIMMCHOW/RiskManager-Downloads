# RiskManager 4.2.2 更新日志

目标版本：ATAS 7.x

## 主要更新

- 新增 ATAS 7.x 独立构建。
- 继续保留 RiskManager 4.2.2 的 Apex / Rithmic 下单兼容改动。
- 默认关闭券商 OCO，减少部分实盘评测连接拒单风险。
- Entry 单不再携带 OCOGroup。
- SL / TP 仅在启用券商 OCO 且存在 TP 时共用 OCOGroup。
- 下单请求和 `OnOrderRegisterFailed` 拒单原因写入授权日志，便于排查实盘连接返回的真实错误。

## 兼容说明

- 本 DLL 只用于 ATAS 7.x。
- ATAS 8.x 请使用 `release-archive\正式版\8.x\RiskManager-4.2.2\RiskManager-4.2.2-ATAS-8.x.dll`。
