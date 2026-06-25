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

## 9. 素材搜索关键词

地图素材：

- pixel forest tileset
- pixel nature tileset
- top down rpg tileset
- pixel village tileset
- pixel house interior tileset
- pixel mountain tileset
- pixel path tileset
- pixel stream tileset
- cozy pixel art tileset

茶铺和室内：

- pixel tea shop
- pixel tavern tileset
- pixel inn interior
- pixel cozy house tileset
- pixel kitchen interior
- pixel shop interior tileset

氛围参考：

- misty pixel art
- cozy pixel art
- warm light pixel art
- forest pixel background
- scenic pixel art

## 10. 第一阶段最少素材列表

第一阶段只需要：

- 1 个主角行走素材
- 1 套草地、森林、石路 tileset
- 1 套木屋或室内素材
- 3 个采集物图标：
  - 茶叶
  - 山泉水
  - 木柴
- 1 套简单 UI 框
- 1 个像素字体
- 1 段环境音乐
- 2 到 3 个音效：
  - 采集
  - 制作
  - 售卖

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
