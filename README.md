# Minecraft Player Analyzer

[![Version](https://img.shields.io/badge/version-V4-blue)](https://github.com/s1791509659/mc-stats-parser)
[![License](https://img.shields.io/badge/license-MIT-green)](https://github.com/s1791509659/mc-stats-parser)

**English** | [简体中文](#简体中文)

A tool to analyze players' stats file in Minecraft — all parsing happens **locally in your browser**, no data is ever uploaded.

> Sorry for being lazy to fully translate the page UI into English (the UI is currently Chinese-first). The README below is fully bilingual.

**Click [Bilibili Tutorial](https://www.bilibili.com/video/BV1MWgzziEHU/) to learn more**

---

## 🌐 Access

### 1. GitHub Pages: [MC Player Analyzer](https://s1791509659.github.io/mc-stats-parser/en_us/) (English) · [中文](https://s1791509659.github.io/mc-stats-parser/)

- English at `/en_us/`, Chinese at the root path
- Available in most areas once you can open GitHub
- Stable and safe

### 2. Retinbox page: [MC Player Analyzer](https://stats.rth1.xyz/en_us/) (English) · [中文](https://stats.rth1.xyz/)

- English at `/en_us/`, Chinese at the root path
- China-network friendly

---

## ✨ Features (V4)

All data is parsed **entirely in your browser** — nothing leaves your computer.

### 📊 Server Overview
- 10+ KPI cards (auto-hides metrics with no data): total playtime, blocks mined/placed, mob kills, deaths, travel distance, and more
- **"Blocks placed" is derived**: vanilla Minecraft has no standalone placed stat — placing a block increments that block's `used` stat. This tool detects the block-like entries of `used` (anything mined by anyone + block-family names + an explicit list) and sums them, so the number is now a meaningful real value instead of a permanent 0
- Server-wide behavior distribution chart (the "custom" counter category is excluded by default to keep the chart readable — toggle it back on anytime)
- Top blocks/items, most active players, death leaderboard
- 20+ automatic "Server Records" (biggest miner, most deaths, longest distance traveled…)
- **Enchantment popularity (Top 12)** and **status-effect usage** across the server

### 👤 Player Profiles
- Avatar, auto-computed title & badge, 12 personal stats
- 8-dimension behavior radar (normalized against the whole server)
- Top statistics bar chart — click a bar to jump straight to the server-wide ranking for that stat
- **41 unlockable achievements** with progress bars
- **Inventory / ender chest / equipment viewer** — real item icons, enchantments and counts, read straight from the player `.dat` (armor & offhand slots of both old and new storage formats)
- **Live player state** — game mode, dimension, coordinates, health, food, XP level, spawn point, current vehicle and more
- **Enchantment summary** for everything the player is carrying
- **Progress timeline** — a cumulative unlock curve (day/week/month granularity picked automatically) plus a day-by-day list, with first/last unlock, active span and busiest-day stats
- **Score card export** — render the whole profile into a shareable PNG (avatar, title, server-wide ranks, KPI grid, rarest advancements)
- One-click copy of a shareable profile summary

### 🏅 Advancements
- Server-wide completion of 118 vanilla advancements, grouped by category (story / nether / end / adventure / husbandry / datapack)
- Per-advancement unlock count, completion share, first & latest achiever
- "In progress" entries — someone is working on it but nobody finished yet

### 🏆 Leaderboard
- 18 preset metrics + full-text search across **all** 5000+ stat keys
- Animated podium (top 3) and top-200 list with share bars
- Export to CSV

### ⚖️ Player Comparison
- Side-by-side radar overlay, head-to-head metric bars
- Detailed diff table (up to 400 rows)
- Zero-value metrics clearly marked as "not recorded in this dataset" instead of a misleading 0

### 📋 Data Table
- Item icons with multi-CDN fallback (text fallback if offline)
- Ownership rarity (how many players have it), per-player share bars
- 5 sort modes, clickable headers, pagination, CSV export

### 🎉 Fun Boards
- 36 fun records (who walked the least? who died the most?)
- Server trivia & auto-generated cold facts
- Rare-item collectors, title wall + overall activity score

### 🧩 Highly Compatible Parser
Works with stats exports from **any** server:
- Any folder layout (`world/stats/`, root, deep nesting…)
- File names as UUID (with/without dashes) or player names
- `usercache.json` anywhere in the zip (any letter case) — player names still shown even without it
- Standard `{"stats":{...}}`, bare stats maps, plugin-wrapped structures
- UTF-8 BOM, numeric strings, modded namespaces (`create:zinc_ore` stays separate)
- Zip-inside-zip, multiple worlds auto-merged per player
- Non-stat files (`advancements/`, `level.dat`…) are skipped automatically — an import report shows exactly what was recognized / skipped / failed

### 🛠 Misc
- Dark / light theme, keyboard shortcuts (`/` `1-6` `R` `T` `P`/`N`/`B` `Esc`)
- **Global player search with avatar autocomplete** — hit `Ctrl`/`⌘` + `K` from anywhere
- URL deep links (share a specific player / leaderboard / comparison)
- Drag & drop import anywhere on the page
- Animated counters, toasts, skeleton loading

---

## 📖 How to use it

1. **Zip your server's `stats` folder**
2. **Add the `usercache.json` file into this zip** (optional, but lets the tool show player names)
3. **Drag this zip file into the website**

That's it — everything else is automatic.

---

## Introduction

A powerful web-based tool designed to analyze and visualize Minecraft player statistics. Upload your JSON or ZIP files containing Minecraft stats data to unlock comprehensive insights into gameplay activities, item usage, and category-based metrics.

Whether you're tracking individual player progress, analyzing server-wide trends, or exploring detailed in-game metrics, this tool turns a dry stats dump into an interactive dashboard.

---

# 简体中文

[English](#minecraft-player-analyzer) | **简体中文**

一个用于分析 Minecraft 玩家统计数据文件的工具 —— 所有解析都在**浏览器本地完成**，数据不会上传到任何服务器。

> 页面 UI 目前以中文为主，README 提供中英双语。

**点击 [B站教程](https://www.bilibili.com/video/BV1MWgzziEHU/) 了解更多**

---

## 🌐 访问入口

### 1. GitHub Pages：[MC Player Analyzer](https://s1791509659.github.io/mc-stats-parser/)（中文页）· [English](https://s1791509659.github.io/mc-stats-parser/en_us/)

- 根路径为中文页，英文页在 `/en_us/`
- 只要能打开 GitHub 就能访问
- 稳定安全

### 2. Retinbox 镜像：[MC Player Analyzer](https://stats.rth1.xyz/)（中文页）· [English](https://stats.rth1.xyz/en_us/)

- 根路径为中文页，英文页在 `/en_us/`
- 国内网络友好

---

## ✨ 功能一览（V4）

所有数据完全在浏览器本地解析，不上传任何内容。

### 📊 服务器总览
- 10+ 张 KPI 卡片（无数据的自动隐藏）：总游戏时长、挖掘/放置方块数、生物击杀、死亡次数、旅行距离等
- **「放置方块」为推算值**：原版 Minecraft 没有独立的放置统计，放置方块会记到该方块的 `used`（使用）统计里。本工具会识别出 `used` 中的方块（全服挖过的物品 + 方块族命名 + 显式清单）并汇总，因此这个数字现在是有意义的真实值，而不是永远的 0
- 全服行为分布环图（默认排除占比过大的「综合统计」，保持图表可读，可一键勾选恢复）
- 最热门方块/物品、最肝玩家榜、死亡榜
- 20+ 项自动评选的「服务器之最」（最强矿工、死亡冠军、旅行最远……）
- **附魔流行度 Top 12** 与 **状态效果** 使用分布

### 👤 玩家档案
- 头像、自动计算的称号徽章、12 项个人数据
- 8 维行为雷达图（相对全服归一化）
- Top 统计条形图 —— 点击柱子直接跳转到该统计项的全服排行榜
- **41 个可解锁成就**，带进度条
- **背包 / 末影箱 / 装备栏查看** —— 真实物品图标、附魔与数量，直接读自玩家 `.dat`（新旧两种存储格式的盔甲与副手槽位都支持）
- **玩家实时状态** —— 游戏模式、所在维度、坐标、生命、饱食度、经验等级、重生点、当前骑乘等
- **附魔汇总** —— 汇总该玩家身上所有附魔
- **进度时间线** —— 累计解锁曲线（自动按天/周/月选粒度）+ 按日期分组的列表，含首次/最近解锁、活跃跨度、最高产的一天
- **战绩卡片导出** —— 把整份档案渲染成可分享的 PNG（头像、称号、全服排名、KPI 网格、最稀有成就）
- 一键复制可分享的档案摘要

### 🏅 成就总览
- 全服 118 项原版成就的完成情况，按分类汇总（剧情 / 下界 / 末地 / 冒险 / 农牧 / 数据包）
- 每项成就的达成人数、完成占比、首位与最近达成者
- 「进行中条目」—— 有人推进但全服尚无人达成

### 🏆 排行榜
- 18 个预设指标 + 对全部 5000+ 统计项的全文搜索
- 领奖台动画（前三名）与前 200 名占比条列表
- 支持导出 CSV

### ⚖️ 玩家对比
- 双色雷达叠加、关键指标对抗条
- 详细差异表（最多 400 行）
- 双方均为 0 的指标会明确标注「数据源未记录」，而不是误导性的 0

### 📋 数据表
- 物品图标（多 CDN 回退，离线时显示文字兜底）
- 稀有度（多少玩家拥有）、占个人比例条
- 5 种排序、点击表头排序、分页、导出 CSV

### 🎉 趣味榜单
- 36 项趣味纪录（谁走得最少？谁死得最勤？）
- 服务器冷知识自动生成
- 稀有物品收藏家、称号墙 + 综合活跃度评分

### 🧩 超强兼容的解析器
兼容**任何服务器**导出的统计数据：
- 任意目录层级（`world/stats/`、根目录、深层嵌套……）
- 文件名可以是 UUID（带/不带横线）或玩家名
- `usercache.json` 在压缩包任意位置（大小写不限）—— 即使没有它也能显示玩家名
- 标准的 `{"stats":{...}}`、裸 stats 映射、插件包裹结构均可
- 兼容 UTF-8 BOM、字符串数字、模组命名空间（`create:zinc_ore` 不会被错误合并）
- 支持压缩包套压缩包，多世界同名玩家自动累加
- 非统计文件（`advancements/`、`level.dat`…）自动跳过，并有导入报告展示识别/跳过/失败明细

### 🛠 其他
- 明暗主题、快捷键（`/` `1-6` `R` `T` `P`/`N`/`B` `Esc`）
- **全局玩家搜索（带头像自动补全）** —— 任意位置按 `Ctrl`/`⌘` + `K` 唤起
- URL 深链接（可分享指定玩家 / 排行榜 / 对比页面）
- 整页任意位置拖拽导入
- 数字滚动动画、Toast 提示、骨架屏加载

---

## 📖 使用方法

1. **把服务器的 `stats` 文件夹压缩成 zip**
2. **把 `usercache.json` 也放进这个压缩包**（可选，放了就能显示玩家名）
3. **把 zip 拖进网页**

就这么简单，剩下的一切自动完成。

---

## 简介

一个强大的网页工具，用于分析与可视化 Minecraft 玩家统计数据。上传包含统计数据的 JSON 或 ZIP 文件，即可获得游戏行为、物品使用、分类统计等全方位洞察。

无论是追踪单个玩家的成长、分析全服趋势，还是探索游戏内的详细数据，这个工具都能把枯燥的统计文件变成交互式仪表盘。
