# Codex 工作流

## 1. 基本原则

Codex 每次只处理一个小任务。

不要一次性要求：

“帮我做完整游戏。”

应该拆成：

- 只做玩家移动
- 只做第一张地图
- 只做采集系统
- 只做背包系统
- 只做制作系统
- 只做售卖系统
- 只做昼夜系统

## 2. 每次使用 Codex 前

进入项目目录：

cd "F:\Godot Projects\sjcp"

查看当前状态：

git status

有稳定改动时先提交：

git add .
git commit -m "save stable state before codex task"

## 3. Codex 应打开的目录

Codex 应该打开这个目录：

F:\Godot Projects\sjcp

这个目录中应该包含：

- project.godot
- AGENTS.md
- README.md
- docs/
- scenes/
- scripts/
- assets/

## 4. 每次给 Codex 的通用要求

在任务末尾追加：

请在完成后按以下格式回答：
1. Changed files
2. What each file does
3. How to test in Godot
4. Possible next step

## 5. 每次 Codex 完成后

先查看 Git 状态：

git status

查看改动：

git diff

然后用 Godot 打开项目测试。

可以尝试：

godot -e

或者手动打开 Godot 编辑器。

## 6. 测试没问题后提交

示例：

git add .
git commit -m "add player movement"

commit 信息根据任务变化。

## 7. 改坏了怎么办

查看提交历史：

git log --oneline

回退到上一个提交：

git reset --hard HEAD~1

只想丢弃未提交改动：

git checkout -- .

## 8. 推荐任务顺序

1. 项目目录结构
2. 玩家移动
3. 第一张地图
4. 采集系统
5. 背包系统
6. 制作系统
7. 售卖系统
8. 昼夜系统
9. 睡觉系统
10. 氛围优化
11. Demo 整理

## 9. 不推荐的 Codex 提问

不要这样问：

“帮我做一个类似星露谷、潜水员戴夫、死亡细胞结合的完整游戏。”

问题：

- 范围太大
- 容易生成复杂代码
- 难以调试
- 容易浪费额度
- 不利于学习

## 10. 推荐的 Codex 提问

推荐这样问：

请只实现 Player.tscn 和 player.gd。

要求：
1. Godot 4。
2. 使用 CharacterBody2D。
3. 2D 俯视角移动。
4. 支持 WASD 和方向键。
5. 添加 Camera2D 跟随。
6. 不要做背包、采集、NPC 或战斗。
7. 完成后告诉我改了哪些文件、脚本挂在哪、如何在 Godot 中测试。
