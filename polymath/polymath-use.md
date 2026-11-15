# 使用

先按 [polymath-install.md](polymath-install.md) 安装，并新开对话。

## 怎样开口

写教案：

```text
/polymath syllabus
我想学 WebRTC，有过一点 WebSocket 经验。
难度：中等
课型：lecture 开、练习 开、前沿实例 关
课程包放在：<某仓库>/docs/courses
目录名用 webrtc-polymath。
载体：markdown + html。
```

语音/互动上课（主入口是对话里的 coach，不是 index.html）：

```text
/polymath coach
课程包在 docs/courses/webrtc-polymath
从课次 1 的 B1 开始；我可能会随时打断。
```

三档难度：简单（扫盲）/ 中等（全面上手）/ 复杂（深入+前沿）。  
课型：`lecture` · `练习` · `前沿实例` 可分别开闭。

## 语音与打断怎么走

1. syllabus 交出带 **beat** 的 `教案.md` 和可选 `labs/**`  
2. 在本对话开 `/polymath coach`（可配合 Cursor 语音）  
3. coach 按 beat 讲 → 你可随时插话 → coach 回退/开 lab/跳课 → 写入 `进度.md`  
4. HTML 只在 coach 叫你看的时候打开（教具）

详见技能内 [live-teaching.md](live-teaching.md)。

## 会得到什么

| 模式 | 产物 |
| --- | --- |
| syllabus | 课包：`清单.md` + 教案（含 beat）+ 载体制品 |
| coach | 对话授课；`进度.md` / 建议 `状态.json` |

## 两个模式的关系

先 syllabus 出包，再 coach 上课。改课次/难度/课型回 syllabus。
