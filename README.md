# 左轮手枪游戏插件 README

## 一、插件概述
基于 `AstrBot` 的群聊左轮手枪游戏插件，玩家可以在群聊中进行左轮手枪射击游戏，支持随机走火事件。

## 二、插件信息
- **插件名称**：revolver_game
- **作者**：长安某
- **关联物品**：左轮手枪插件
- **版本号**：1.0.0

## 三、功能介绍

### 1. 装填子弹
玩家可以使用 `装填 [子弹数量]` 命令向 6 弹匣的左轮手枪中装填实弹。
- **参数说明**：
  - `[子弹数量]`：可选参数，必须为 1 到 6 之间的整数，默认值为 1。
- **示例**：
  - `装填`：默认装填 1 发实弹。
  - `装填 3`：装填 3 发实弹。

### 2. 射击
玩家使用 `射爆` 命令进行射击。
- 如果当前弹仓为实弹，玩家会被击中并被禁言 60 秒，同时游戏会输出相应的击中提示信息。
- 如果当前弹仓为空弹，游戏会输出空枪提示信息，玩家可继续射击。
- 当弹匣内的所有实弹都射出后，游戏结束，玩家可以再次装填开始新游戏。

### 3. 随机走火
在群聊中，有一定概率（默认为 0.005）触发随机走火事件。当走火发生时，会输出走火相关的提示信息，并且走火击中的玩家会被禁言 60 秒。

### 4. 走火功能开关
- `走火开`：开启本群的左轮手枪走火功能。
- `走火关`：关闭本群的左轮手枪走火功能。

### 5. 游戏超时处理
如果在装填子弹后 60 秒内没有玩家继续射击，游戏会自动结束，并输出相应的超时提示信息。

## 四、更新
