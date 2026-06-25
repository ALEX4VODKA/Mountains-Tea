
# Codex 任务 Prompt 集合

本文件用于保存适合直接复制给 Codex 的任务提示词。

使用原则：

* 每次只让 Codex 做一个系统。
* 不要一次性让 Codex 做完整游戏。
* 每次任务开始前先提交 Git。
* 每次任务完成后在 Godot 里测试。
* 测试通过后再提交 Git。

---

## 通用结尾格式

每次给 Codex 的任务后面都可以加：

```text
请在完成后按以下格式回答：
1. Changed files
2. What each file does
3. How to test in Godot
4. Possible next step
```

---

## 任务 0：阅读项目文档

```text
请阅读 AGENTS.md、README.md 和 docs/design.md，理解当前 Godot 4 项目“Mountain Tea House / 山间茶铺”的方向。

不要修改任何文件。
只总结：
1. 项目目标
2. 第一阶段功能范围
3. 当前应该优先做什么
4. 你会遵守哪些开发限制
```

---

## 任务 1：建立基础目录结构

```text
请为这个 Godot 4 项目检查并完善基础目录结构。

要求：
1. 目录结构要适合一个 2D 俯视角像素风休闲探索游戏。
2. 项目名为“Mountain Tea House / 山间茶铺”。
3. 不要写具体玩法代码。
4. 不要引入复杂架构。
5. 不要创建无关文件。

请在完成后按以下格式回答：
1. Changed files
2. What each file does
3. How to test in Godot
4. Possible next step
```

---

## 任务 2：玩家移动系统

```text
请只实现 Godot 4 的玩家移动系统。

要求：
1. 创建 scenes/player/Player.tscn。
2. 创建 scripts/player/player.gd。
3. 使用 CharacterBody2D。
4. 实现 2D 俯视角移动。
5. 支持 WASD 和方向键。
6. 添加 Camera2D 跟随玩家。
7. 使用简单占位图形即可。
8. 代码保持简单、适合初学者理解。
9. 不要实现背包、战斗、采集、NPC 或其他系统。

请在完成后按以下格式回答：
1. Changed files
2. What each file does
3. How to test in Godot
4. Possible next step
```

---

## 任务 3：第一张主地图

```text
请创建第一张测试地图 scenes/world/TeaHouseMap.tscn。

要求：
1. 这是一个 2D 俯视角地图。
2. 地图包含：
   - 茶铺主体区域
   - 门前小路
   - 一小片树林
   - 一处溪流或取水点
3. 暂时使用占位色块或简单节点，不依赖真实素材。
4. 加入 Player 实例。
5. 预留 TileMap / TileMapLayer 节点。
6. 加入基础边界碰撞。
7. 不要制作复杂玩法系统。
8. 不要引入真实素材。

请在完成后按以下格式回答：
1. Changed files
2. What each file does
3. How to test in Godot
4. Possible next step
```

---

## 任务 4：采集物系统

```text
请实现一个最小可用的采集系统。

要求：
1. 创建 scenes/interactables/Collectible.tscn。
2. 创建 scripts/interactables/collectible.gd。
3. 玩家靠近可显示“按 E 采集”。
4. 按 E 后物品消失。
5. 支持三种资源：
   - tea_leaves
   - spring_water
   - firewood
6. 先用简单信号或方法把采集结果发送给背包系统。
7. 不做复杂动画。
8. 不做刷新系统。

请在完成后按以下格式回答：
1. Changed files
2. What each file does
3. How to test in Godot
4. Possible next step
```

---

## 任务 5：最小背包系统

```text
请实现一个最小可用的 Inventory 系统。

要求：
1. 创建 scripts/systems/inventory.gd。
2. 支持添加物品。
3. 支持记录物品数量。
4. 创建 scenes/ui/HUD.tscn。
5. 创建 scripts/ui/hud.gd。
6. 在 HUD 左上角显示物品名和数量。
7. 只显示文字，不做格子背包。
8. 不做拖拽，不做分页，不做装备栏。
9. 与采集系统联动。

请在完成后按以下格式回答：
1. Changed files
2. What each file does
3. How to test in Godot
4. Possible next step
```

---

## 任务 6：制作系统

```text
请实现一个最小可用的制作系统。

要求：
1. 创建 CraftingStation 交互点。
2. 玩家靠近制作点按 E 可以制作。
3. 第一版只支持一个配方：
   tea_leaves + spring_water = simple_tea
4. 制作时扣除材料。
5. 制作后增加 simple_tea。
6. 材料不足时显示提示。
7. 界面尽量简单。
8. 不做复杂菜单系统。

请在完成后按以下格式回答：
1. Changed files
2. What each file does
3. How to test in Godot
4. Possible next step
```

---

## 任务 7：售卖系统

```text
请实现一个最小可用的售卖系统。

要求：
1. 在茶铺柜台设置售卖交互点。
2. 玩家靠近后按 E 可以卖出 simple_tea。
3. 卖出后背包减少 simple_tea。
4. 金币增加。
5. HUD 中显示金币。
6. 第一版只支持卖出 simple_tea。
7. 不做复杂经济系统。
8. 不做价格浮动。

请在完成后按以下格式回答：
1. Changed files
2. What each file does
3. How to test in Godot
4. Possible next step
```

---

## 任务 8：昼夜系统

```text
请实现一个最小可用的昼夜系统。

要求：
1. 创建 scripts/systems/day_night_system.gd。
2. 增加一个时间变量。
3. 随时间推进，画面颜色逐渐变化。
4. 建议使用 CanvasModulate 或类似简单方式。
5. 白天、黄昏、夜晚要有明显区别。
6. 不做复杂日历系统。
7. 不做天气系统。

请在完成后按以下格式回答：
1. Changed files
2. What each file does
3. How to test in Godot
4. Possible next step
```

---

## 任务 9：睡觉进入下一天

```text
请实现睡觉进入下一天的交互。

要求：
1. 创建 Bed 交互点。
2. 玩家靠近床边按 E 可以睡觉。
3. 睡觉后进入下一天。
4. 保留背包和金币。
5. 可以重置当天时间到早晨。
6. 不做复杂日历系统。
7. 不做存档系统。

请在完成后按以下格式回答：
1. Changed files
2. What each file does
3. How to test in Godot
4. Possible next step
```

