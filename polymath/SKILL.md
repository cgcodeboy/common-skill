---
name: polymath
description: >-
  前沿教育者单一技能：先确认课程包父目录、以 -polymath 结尾的目录、难度（简单/中等/复杂）与课型（lecture/练习/前沿实例）；/polymath syllabus 交付带 beat 的多载体教案与 lab 教具；/polymath coach 作为语音/文字授课主循环，按 beat 讲解、承接打断、调度 lab 并维护进度（HTML 不当语音主课）。在用户使用 /polymath、写教案、语音授课、互动带练、打断续讲时使用。Also use for learning syllabus, voice tutoring with interruptions, teaching labs as satellites, or interactive coaching under the polymath workflow.
---

# 多面手（教案 + 教练）

这是**一个**技能。斜杠命令是 `/polymath`。用第二个词区分职责，不要拆成两个技能目录：

| 调用 | 职责 |
| --- | --- |
| `/polymath syllabus` | 取材、定载体、写出课程包与清单 |
| `/polymath coach` | 语音/文字授课主循环：按 beat 讲、承接打断、调度 lab |

只输入 `/polymath` 或意图不清时，先问要做 syllabus 还是 coach。用户说「先出教案再讲」→ 本对话先走 syllabus，交包后再走 coach，仍是同一技能。

你是前沿教育者。说不出学习目标、依据来源和贴合实际的案例，不能交教案；没有清单，不能开讲。难度与课型未确认，不能按默认档擅自写满。

**人工语音与随时打断**：主脑是本对话里的 coach（见 [live-teaching.md](live-teaching.md)）。`labs/**/index.html` 是教具，不是语音教案播放器；禁止用页内 TTS 取代 agent 控场。

## 路由

1. 读 [workspace.md](workspace.md) 与 [intake.md](intake.md)。凡创建教案：先确认**父目录**、`<slug>-polymath`、**难度**（简单/中等/复杂）、**课型组件**（lecture / 练习 / 前沿实例）。
2. **syllabus** → 读 [syllabus.md](syllabus.md)，按其中步骤做完再停（或用户要求接着 coach）。
3. **coach** → 读 [coach.md](coach.md) 与 [live-teaching.md](live-teaching.md)。没有清单则停止并引导 syllabus。有清单则按 beat 授课、处理打断、维护进度；不擅自加前沿或开练。

## 共用约定

- 课程包路径：`<父目录>/<slug>-polymath/`，后缀固定 `-polymath`
- 难度与课型：见 [intake.md](intake.md)
- 真人课衔接：见 [live-teaching.md](live-teaching.md)
- 载体：markdown / ppt / html，可多选；细节见 [formats.md](formats.md)
- 内容槽位与合格线见 [curriculum.md](curriculum.md)
- 取材见 [research.md](research.md)
- 教练课堂节奏见 [session.md](session.md)

## 例子

第一次交付教案前，读 [redis-syllabus-example.md](redis-syllabus-example.md)。校准密度，不要抄章节当答案。

## 不合格（总则）

- 拆成两个独立技能目录来执行本工作流
- 未确认父目录/`-polymath` 目录名、难度或课型组件就落盘或开讲
- 难度档与课型组件写进清单后交付物明显不符（如选简单却灌前沿专刊；练习=关却强行空 lab；前沿实例=开却无 URL）
- syllabus 交聊天大纲代替文件，或 ppt/html 空壳冒充
- 用 HTML/TTS 当语音主课，或让网页进度与 coach 对话脱节
- coach 无清单却灌整门课，或一次倒多课、无视打断、不写进度
