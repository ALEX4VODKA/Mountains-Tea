# TODO：山间茶铺

## Milestone 0：项目初始化

- [ ] 确认 Godot 项目可以正常打开
- [ ] 设置渲染器为 Compatibility
- [ ] 设置像素纹理过滤为 Nearest
- [ ] 设置窗口分辨率为 640x360
- [ ] 创建基础目录结构
- [ ] 创建 README.md
- [ ] 创建 AGENTS.md
- [ ] 创建 docs 文档
- [ ] 初始化 Git
- [ ] 完成初始提交

## Milestone 1：玩家移动

- [ ] 创建 Player.tscn
- [ ] 创建 player.gd
- [ ] 使用 CharacterBody2D
- [ ] 实现 WASD 移动
- [ ] 实现方向键移动
- [ ] 添加 Camera2D 跟随
- [ ] 在测试场景中验证移动

## Milestone 2：第一张地图

- [ ] 创建 TeaHouseMap.tscn
- [ ] 创建茶铺区域
- [ ] 创建门前小路
- [ ] 创建树林区域
- [ ] 创建溪流或取水点
- [ ] 加入 Player 实例
- [ ] 添加地图边界
- [ ] 设置主场景

## Milestone 3：采集系统

- [ ] 创建 Collectible.tscn
- [ ] 创建 collectible.gd
- [ ] 实现玩家靠近检测
- [ ] 实现“按 E 采集”
- [ ] 支持 tea_leaves
- [ ] 支持 spring_water
- [ ] 支持 firewood
- [ ] 采集后物品消失
- [ ] 采集结果能传给背包系统

## Milestone 4：背包系统

- [ ] 创建 inventory.gd
- [ ] 支持添加物品
- [ ] 支持记录物品数量
- [ ] 创建 HUD.tscn
- [ ] 创建 hud.gd
- [ ] 在 HUD 显示物品数量
- [ ] 采集后 HUD 自动刷新

## Milestone 5：制作系统

- [ ] 创建 CraftingStation.tscn
- [ ] 创建 crafting_station.gd
- [ ] 玩家靠近制作点后可交互
- [ ] 实现 simple_tea 配方
- [ ] 制作时扣除 tea_leaves
- [ ] 制作时扣除 spring_water
- [ ] 制作后增加 simple_tea
- [ ] 制作失败时显示材料不足

## Milestone 6：售卖系统

- [ ] 创建 SellingCounter.tscn
- [ ] 创建 selling_counter.gd
- [ ] 玩家靠近柜台后可交互
- [ ] 支持卖出 simple_tea
- [ ] 卖出后扣除 simple_tea
- [ ] 卖出后增加金币
- [ ] HUD 显示金币

## Milestone 7：昼夜与睡觉

- [ ] 创建 day_night.gd
- [ ] 实现时间变量
- [ ] 实现画面颜色变化
- [ ] 创建 Bed.tscn
- [ ] 创建 bed.gd
- [ ] 玩家靠近床后可睡觉
- [ ] 睡觉后进入下一天
- [ ] 保留背包和金币

## Milestone 8：氛围优化

- [ ] 加入茶铺暖光
- [ ] 加入简单雾气
- [ ] 加入溪流动画
- [ ] 加入树叶或草地装饰
- [ ] 加入背景音乐
- [ ] 加入交互音效
- [ ] 优化 UI 显示

## Milestone 9：第一个可玩 Demo

- [ ] 创建开始菜单
- [ ] 创建暂停菜单
- [ ] 加入简单玩法说明
- [ ] 完成 5 到 10 分钟体验流程
- [ ] 导出 Windows 版本
- [ ] 在 README 中记录运行方式