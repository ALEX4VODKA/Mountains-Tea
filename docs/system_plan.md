# 《山间茶铺》第一阶段系统设计文档

本文档只整理第一阶段最小可玩版本需要的系统边界，不包含代码实现。

## Inventory

### 作用

记录玩家当前拥有的物品数量，用于采集、制作、售卖和界面显示。

### 最少需要的数据

- `tea_leaves` 数量
- `spring_water` 数量
- `firewood` 数量
- `simple_tea` 数量
- `money` 金钱数量

### 关联的场景或脚本

- `scripts/systems/inventory.gd`
- `scripts/player/player.gd`
- `scripts/ui/inventory_ui.gd`
- `scenes/ui/inventory_ui.tscn`

### 第一版不做什么

- 不做背包格子限制。
- 不做物品重量。
- 不做物品分类页。
- 不做拖拽整理。
- 不做复杂存档。

## Collectible

### 作用

让玩家在地图上靠近资源点并互动，获得基础资源。

### 最少需要的数据

- 资源类型：`tea_leaves`、`spring_water`、`firewood`
- 每次采集获得的数量
- 是否已经被采集
- 可交互提示文本

### 关联的场景或脚本

- `scenes/interactables/collectible.tscn`
- `scripts/interactables/collectible.gd`
- `scripts/player/player.gd`
- `scripts/systems/inventory.gd`

### 第一版不做什么

- 不做随机掉落。
- 不做采集工具。
- 不做资源品质。
- 不做资源刷新计时。
- 不做复杂采集动画。

## Crafting

### 作用

让玩家在茶铺或制作点把基础资源合成为可售卖物品。

### 最少需要的数据

- 配方输入：`tea_leaves` x 1、`spring_water` x 1
- 配方输出：`simple_tea` x 1
- 制作是否成功
- 制作提示文本

### 关联的场景或脚本

- `scenes/interactables/crafting_station.tscn`
- `scripts/interactables/crafting_station.gd`
- `scripts/systems/inventory.gd`
- `scripts/ui/inventory_ui.gd`

### 第一版不做什么

- 不做多个配方列表。
- 不做制作时间。
- 不做制作失败概率。
- 不做配方解锁。
- 不做复杂制作界面。

## Selling

### 作用

让玩家把制作出的 `simple_tea` 卖给访客或售卖点，并获得金钱。

### 最少需要的数据

- 可售卖物品：`simple_tea`
- 单价
- 当前拥有数量
- 售卖后增加的 `money`
- 售卖提示文本

### 关联的场景或脚本

- `scenes/interactables/selling_spot.tscn`
- `scripts/interactables/selling_spot.gd`
- `scripts/systems/inventory.gd`
- `scripts/ui/inventory_ui.gd`

### 第一版不做什么

- 不做讨价还价。
- 不做顾客偏好。
- 不做订单系统。
- 不做价格波动。
- 不做复杂 NPC 对话树。

## DayNight

### 作用

表现一天的时间变化，提供白天探索、晚上回屋睡觉、进入下一天的基础循环。

### 最少需要的数据

- 当前天数
- 当前时间阶段：白天、傍晚、夜晚
- 时间推进速度
- 是否允许睡觉
- 睡觉后的新一天状态

### 关联的场景或脚本

- `scripts/systems/day_night.gd`
- `scenes/interactables/bed.tscn`
- `scripts/interactables/bed.gd`
- `scenes/world/world.tscn`
- `scripts/ui/day_night_ui.gd`

### 第一版不做什么

- 不做真实分钟级时间系统。
- 不做天气系统。
- 不做季节系统。
- 不做 NPC 日程。
- 不做复杂灯光和阴影模拟。
