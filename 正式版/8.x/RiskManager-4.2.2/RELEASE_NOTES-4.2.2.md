# RiskManager 4.2.2 发布说明

这是适用于 ATAS 8.x 的 RiskManager 4.2.2 正式版。

本版本重点是将 ATAS 8.x 产物与 ATAS 7.x 产物分开归档，同时保留 4.2.2 对 Apex / Rithmic 下单场景的兼容补丁。正式 DLL 已通过 .NET Reactor 保护，文件名不带 `protected` 字样。

## 下载文件

```text
RiskManager-4.2.2.dll
```

## 安装位置

```text
%AppData%\ATAS\Strategies\
```

## 注意事项

- 请确认本机使用的是 ATAS 8.x。
- 如果升级后出现授权机器码不匹配，请在 Trading Hub 后台重置该授权的 `machine_hash` 后重新验证。
- 实盘使用前请先在模拟盘或回放环境完整测试。
