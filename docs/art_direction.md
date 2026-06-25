# 美术方向：山间茶铺

## 1. 总体方向

《山间茶铺》的美术方向是：

2D 俯视角像素风  
+ 自然风景  
+ 温暖茶铺  
+ 轻 2.5D 氛围

第一阶段不强依赖武侠素材。优先使用通用高质量像素自然风景资源，先完成一个稳定可玩的 demo。后续再通过少量中式元素增强“山间茶铺”的气质。

## 2. 视觉关键词

英文关键词：

- pixel art
- cozy
- top-down
- scenic
- nature
- forest
- mountain
- stream
- tea house
- wooden cabin
- warm light
- mist
- quiet
- relaxing
- small shop

中文关键词：

- 像素风
- 俯视角
- 风景好
- 自然
- 森林
- 山间
- 溪流
- 木屋
- 茶铺
- 暖光
- 雾气
- 安静
- 治愈
- 小店

## 3. 场景关键词

第一版主要场景：

- 山间茶铺
- 门前石板路
- 小树林
- 溪流或水井
- 采集区域
- 茶铺室内
- 睡觉点

## 4. 场景构图建议

茶铺门前要有层次：

- 近景：草、木桶、石阶、小花、木牌
- 中景：茶铺、柜台、桌椅、路灯
- 远景：树林、山坡、雾气、溪流

地图不要太空。尽量避免大面积纯色地面。

可以用这些元素打散画面：

- 草丛
- 石头
- 树影
- 小路边缘
- 落叶
- 木桶
- 木牌
- 小花
- 茶桌
- 灯笼
- 竹子
- 水边石块

## 5. 色彩方向

推荐色彩：

- 山间：青灰、墨绿、竹绿
- 草地：低饱和绿色
- 茶铺：木色、暖黄、暗红
- 黄昏：橙色、紫灰、深蓝
- 雾气：灰白、浅蓝灰

避免：

- 过于刺眼的高饱和颜色
- 大量纯黑边
- 风格混乱的素材混搭
- 分辨率不统一的像素素材混用

## 6. 光影方向

核心目标：温暖、安静、有归属感。

建议使用：

- 茶铺门口暖光
- 室内灯笼或火炉暖光
- 傍晚整体偏橙色
- 夜晚整体偏蓝灰色
- 山林区域有轻雾
- 小溪附近颜色略冷

Godot 中可逐步使用：

- CanvasModulate
- PointLight2D
- LightOccluder2D
- GPUParticles2D 或 CPUParticles2D
- Parallax2D

## 7. 轻 2.5D 表现

轻 2.5D 不是做真 3D，而是在 2D 中做空间感。

可以通过以下方式实现：

- YSort 或 Y 轴排序
- TileMapLayer 分层
- 前景树木遮挡玩家
- 远山或远树视差背景
- 地面阴影
- 雾气粒子
- 暖光和夜色

## 8. UI 风格方向

UI 要简单、清晰、温暖。

适合：

- 木质边框
- 纸张感面板
- 暖色按钮
- 简单像素字体
- 小图标加数字

第一版 UI 不要复杂：

- 左上角显示背包
- 右上角显示金币和时间
- 交互时显示“按 E”
- 制作和售卖面板保持最小化

## 9. 第一阶段美术资源搜索清单

第一阶段搜索重点不是“武侠”，而是“通用高质量像素自然风景 + 温暖小店”。先保证画面统一、可读、容易落地，再通过茶壶、木牌、灯笼、竹子、石板路等小物件补充中式气质。

### 地图 tileset 搜索关键词

优先搜索：

- top down pixel forest tileset
- top down pixel nature tileset
- cozy pixel forest tileset
- pixel art forest tileset
- pixel grass path tileset
- pixel stone path tileset
- pixel stream tileset
- pixel river tileset top down
- pixel mountain nature tileset
- top down RPG nature tileset
- 16x16 pixel nature tileset
- 32x32 pixel nature tileset

组合搜索：

- cozy top down forest tileset
- pixel forest village tileset
- pixel cabin forest tileset
- pixel mountain forest tileset
- pixel nature tileset stream path
- RPG maker style forest tileset pixel

需要覆盖的地图元素：

- 草地
- 草丛
- 树和树冠
- 石板路或泥路
- 石头
- 小花
- 溪流或水井
- 木桥或踏石
- 木屋外墙
- 暖色窗光或灯光装饰

### 茶铺室内素材关键词

优先搜索：

- pixel cozy house interior tileset
- pixel cabin interior tileset
- pixel shop interior tileset
- pixel tavern interior tileset
- pixel inn interior tileset
- pixel kitchen interior tileset
- pixel wooden furniture tileset
- top down pixel interior tileset
- cozy pixel room tileset

补充搜索：

- pixel tea table
- pixel tea cup
- pixel teapot
- pixel wooden counter
- pixel shelf tileset
- pixel fireplace interior
- pixel paper lantern
- pixel warm light interior

需要覆盖的室内元素：

- 木地板
- 墙面
- 柜台
- 桌椅
- 货架
- 茶具或可替代的小餐具
- 床或睡觉点
- 暖灯、炉火或窗光

### 主角素材关键词

优先搜索：

- top down pixel character
- top down pixel character sprite
- pixel character 4 direction walk
- pixel RPG character walking spritesheet
- cozy game pixel character
- farmer pixel character top down
- villager pixel character sprite
- adventurer pixel character top down

可选气质关键词：

- pixel character straw hat
- pixel character apron
- pixel character simple clothes
- pixel character village outfit

主角素材最低要求：

- 至少 4 方向行走：上、下、左、右
- 像素尺寸和地图 tileset 接近，优先 16x16、24x24、32x32
- 轮廓清楚，不依赖复杂动作
- 第一阶段不需要攻击、技能、装备动画

### UI 素材关键词

优先搜索：

- pixel UI pack
- cozy pixel UI
- pixel RPG UI
- pixel inventory UI
- pixel icon pack
- pixel item icons
- pixel fantasy UI
- pixel wood UI
- pixel paper UI
- pixel button UI

资源图标搜索：

- pixel tea leaves icon
- pixel water bottle icon
- pixel water drop icon
- pixel firewood icon
- pixel tea cup icon
- pixel coin icon
- pixel clock icon
- pixel backpack icon

UI 最低需求：

- 背包面板背景
- 物品格子
- 按钮
- 金币图标
- 时间或昼夜图标
- 交互提示框
- 茶叶、山泉水、木柴、简单茶图标

### 音效和音乐关键词

环境音乐：

- cozy pixel game music
- relaxing forest game music
- peaceful village game music
- cozy shop game music
- calm acoustic game loop
- relaxing nature loop music
- tea house ambience music
- peaceful mountain ambience

环境音：

- forest ambience loop
- stream ambience loop
- birds ambience loop
- night ambience loop
- cozy fireplace ambience

音效：

- pixel collect sound
- item pickup sound
- crafting sound effect
- coin sound effect
- shop bell sound effect
- UI click sound pixel
- sleep sound effect
- water collect sound
- wood pickup sound

音频最低要求：

- 1 段可循环的白天环境音乐
- 1 个采集音效
- 1 个制作音效
- 1 个售卖或金币音效
- 可选：溪流环境音、夜晚环境音、UI 点击音效

## 10. 第一阶段最少素材列表

第一阶段不要追求素材数量多。最少下载这些素材即可开始替换占位图：

1. 主角行走 spritesheet
   - 用途：玩家移动
   - 最低要求：4 方向行走
   - 可接受风格：村民、采集者、店主、旅行者

2. 自然地图 tileset
   - 用途：茶铺外部地图
   - 最低要求：草地、树、石路、石头、花草
   - 优先带有：溪流、水边石块、木桥、山地边缘

3. 木屋或茶铺外观 tileset
   - 用途：茶铺建筑外观
   - 最低要求：木墙、屋顶、门、窗
   - 可替代方案：通用木屋、小屋、村庄建筑素材

4. 室内 tileset
   - 用途：茶铺室内、制作点、售卖点、睡觉点
   - 最低要求：木地板、墙、柜台、桌椅、货架、床
   - 可替代方案：cozy house、inn、tavern、shop interior

5. 物品图标小包
   - 用途：背包和制作显示
   - 最低要求：
     - tea_leaves：茶叶
     - spring_water：水滴、水瓶或泉水
     - firewood：木柴
     - simple_tea：茶杯或茶壶
     - coin：金币

6. 简单像素 UI 包
   - 用途：背包、金币、时间、提示、制作和售卖面板
   - 最低要求：面板、格子、按钮、提示框
   - 风格建议：木质、纸张、暖色、低饱和

7. 像素字体
   - 用途：UI 文本
   - 最低要求：英文和数字清晰
   - 如果要显示中文，必须确认字体支持中文字符

8. 白天环境音乐
   - 用途：外部探索和茶铺氛围
   - 最低要求：可循环、安静、自然、不过于史诗

9. 基础音效包
   - 用途：交互反馈
   - 最低要求：
     - 采集
     - 制作
     - 售卖或金币
     - UI 点击可选

## 11. 素材使用原则

可以用作正式资源：

- 自制素材
- CC0 素材
- 明确允许使用的免费素材
- 已购买且授权清楚的素材

只作为参考，不放进正式项目：

- Steam 游戏截图
- B 站视频截图
- Pinterest 图片
- 小红书图片
- 其他游戏拆包素材
- 授权不清楚的 AI 图包

## 12. 后续中式感增强方式

不需要一开始强找武侠素材。

后续可以通过这些元素增强气质：

- 竹林
- 灯笼
- 木牌
- 茶壶
- 茶杯
- 石板路
- 木桌
- 斗笠旅人
- 山间小桥
- 远处山影
- 暖色窗光
