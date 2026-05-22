# RiskManager 4.2-D 更新日志

## 版本

RiskManager 4.2-D

## 状态

内部开发阶段版本。

## 重点

风险预设按钮、订单按钮显示开关、Cancel 订单和仓位处理增强，以及 HUD 模块顺序修正。

## 变更

- 新增固定风险预设按钮。
- 新增风险预设启用 / 禁用设置。
- 新增风险预设金额设置。
- 风险预设模块接入 HUD 模块化和模块排序。
- Risk Preset Module 现在是默认第一个 HUD 模块。
- HUD 模块默认排序现在使用 1-7。
- HUD Modules 设置组中新增并置顶 Show Risk Preset Module。
- Risk Preset Module 参与 HUD 模块排序和 hit-test。
- 新增订单按钮显示开关。
- 新增 MKT / BID/ASK / LMT / STP / Cancel 按钮显示控制。
- 新增 Cancel Button Mode。
- 将“当前品种全部挂单”范围升级为“当前品种订单和仓位”。
- 新增可选的当前账户、当前品种订单撤销和仓位关闭功能。
- 新增 Cancel 二次点击确认流程。
- 新增撤单安全检查。
- RiskManager Orders Only 默认只匹配当前策略实例创建的订单。
- 授权无效时允许清空本地选择状态，但禁止撤真实订单或处理仓位。
- 修复 Cancel 关闭仓位时同步等待 ATAS 异步接口导致图表卡死的问题。
- 订单和仓位处理现在使用非阻塞异步流程，并防止重复触发。

## 说明

此阶段不开发账户百分比风险模式，不修改 Supabase 后端，不重写核心下单状态机。
