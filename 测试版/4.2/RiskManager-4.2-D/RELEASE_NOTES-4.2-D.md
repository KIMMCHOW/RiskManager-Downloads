# RiskManager 4.2-D 发布说明

RiskManager 4.2-D 是 RiskManager 4.2 开发周期中的内部阶段版本。

此版本新增风险预设按钮、订单按钮显示开关，并增强 Cancel 按钮行为。本次修正后，风险预设模块默认显示在 HUD 最上方，Cancel 的当前品种范围已从“全部挂单”升级为“订单和仓位”。

## HUD 模块顺序

默认 HUD 模块顺序为：

1. Risk Preset Module
2. Account Module
3. Tick Module
4. Risk Module
5. Price Module
6. Order Module
7. Status Module

默认 Order 值使用 1-7。用户仍然可以在 HUD Module Order 设置组中修改排序。Order 相同的情况下，会使用上述默认顺序作为稳定的 tie-breaker。

## 风险预设按钮

默认显示四个固定金额风险按钮：

- 200
- 500
- 1000
- 2000

每个按钮都可以单独启用 / 禁用，也可以修改金额。点击按钮后，会把当前 SL Amount 设置为对应金额。如果 Entry 和 Stop 已经选择完成，会立即重新计算 Tick Distance、Auto Qty 和 RR Target。

## 设置面板

- HUD Modules 设置组中，Show Risk Preset Module 排在第一个。
- HUD Module Order 设置组中，Risk Preset Module Order 排在第一个。
- Risk Presets 设置组中，四组预设按钮按 Enable / Amount 成对排列。

## 订单按钮显示开关

Order Module 中的按钮可以单独控制显示：

- MKT
- BID/ASK
- LMT
- STP
- Cancel

隐藏按钮只影响 HUD 显示和点击区域，不删除内部下单能力。

## Cancel 模式

Cancel 有两种模式：

1. `Clear RiskManager State Only`
   - 只清空当前 RiskManager 操作流程。
   - 不撤市场中的真实订单。

2. `Clear State + Cancel Orders and Position`
   - 清空当前操作流程。
   - 可撤销当前账户、当前图表品种下的未成交订单。
   - 当 Cancel Scope 选择当前品种订单和仓位时，会调用 ATAS 的持仓关闭接口处理当前图表品种仓位。
   - 默认需要 3 秒内二次点击确认。

默认模式是 `Clear RiskManager State Only`。

## 4.2-D 修正

Cancel 处理订单和仓位时不再同步等待 ATAS 的异步持仓关闭接口，避免点击 Cancel 后图表或 ATAS 卡死。订单撤销和仓位处理现在会以非阻塞异步流程执行，并防止重复触发。

## 风险提示

- 当前品种订单和仓位模式会撤销未成交订单，并请求关闭当前图表品种仓位。
- 默认 Cancel Scope 只撤当前 RiskManager 策略实例创建的订单。
- 如果切换为当前品种订单和仓位范围，可能会撤掉用户手动挂出的当前品种订单，并处理当前品种已有仓位。
- 仓位关闭依赖 ATAS 官方 `ClosePosition` 流程，不直接绕过 ATAS 交易接口。
- 使用前必须确认当前账户和图表品种正确。
- 实盘前必须先在模拟环境测试。
