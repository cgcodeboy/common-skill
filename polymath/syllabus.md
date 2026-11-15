# 模式：syllabus（写教案）

触发：`/polymath syllabus`，或用户明确要求写教案 / PPT / HTML 课包 / 学习路径且尚未要开讲。

本模式只交课程包与清单。讲解是 [coach.md](coach.md)。交完后提示：`/polymath coach`。

## 行为准则

1. 目标写成可检验能力；写不出先假设并标明待确认。
2. **先落盘位置**：[workspace.md](workspace.md) → 确认父目录与 `<slug>-polymath` → 再 `mkdir`。
3. **再定难度与课型**：[intake.md](intake.md)。必须确认：简单 / 中等 / 复杂；以及 lecture、练习、前沿实例各开或关。
4. **再定载体**：[formats.md](formats.md)。未指定则问；结合课型默认（练习开→倾向 html；lecture 开→markdown，要投影再加 ppt）。
5. 真实检索：[research.md](research.md)。权威文档 + 教程 + ≥2 可打开仓库（GitLab 优先）；前沿实例开则另加前沿源。
6. 课次数量与深度跟难度走，见 [curriculum.md](curriculum.md)；槽位按课型裁剪。lecture=开时讲解顺序必须拆成 **beat**，供 coach 语音课打断回点（[live-teaching.md](live-teaching.md)）。
7. html 是教具不是语音主课；禁止交付「页内 TTS 自动授课站点」充 lecture。
8. 禁止聊天大纲代替文件；禁止文本提纲冒充 `.pptx`；禁止空 html 壳。
9. 已有包则先读 `清单.md` 再改；改难度/课型要重写课次地图受影响部分。

## 步骤

1. 确认领域、父目录、`<slug>-polymath`、先验、**难度**、**课型组件**（lecture / 练习 / 前沿实例）、目标、载体。目录、难度、三项组件必须得到确认（或复述用户已声明的内容请其点头）。
2. 按难度与课型取材；聊天里给来源摘要。
3. 定课次地图与槽位落点（简单偏导览，中等主干，复杂加前沿专次）。
4. 写 `清单.md`（含难度与课型字段）与已选载体制品。
5. 对照 curriculum 合格线自检后交付。
6. 给出课程包路径与 `/polymath coach` 开讲提示。

## 交付

```text
<父目录>/<slug>-polymath/清单.md
```

加已选载体文件。可选 `来源.md`。
