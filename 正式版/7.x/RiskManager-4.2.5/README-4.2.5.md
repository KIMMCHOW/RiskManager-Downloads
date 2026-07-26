# RiskManager 4.2.5 使用说明 / RiskManager 4.2.5 Guide

## 安装 / Installation

- 下载与当前 ATAS 版本匹配的 DLL：`RiskManager-4.2.5-ATAS-7.x.dll`。
  Download the DLL that matches your ATAS version: `RiskManager-4.2.5-ATAS-7.x.dll`.
- 将 DLL 放入 ATAS 策略目录：`%AppData%\ATAS\Strategies\`。
  Copy the DLL into the ATAS strategies folder: `%AppData%\ATAS\Strategies\`.
- 重启 ATAS，并在图表中添加 RiskManager Chart Strategy。
  Restart ATAS and add RiskManager Chart Strategy on the chart.

## 说明 / Notes

- 本包适用于 ATAS 7.x，目标框架为 `net8.0-windows`。
  This package is for ATAS 7.x and targets `net8.0-windows`.
- 不要混用不同 ATAS 版本的 DLL。
  Do not mix DLLs across ATAS versions.
- 正式交易前，请先在模拟账户或回放环境中验证完整下单流程。
  Before live trading, verify the full order workflow in simulation or replay.
