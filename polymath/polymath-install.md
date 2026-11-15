# 安装

源文件是本目录。这是**一个**技能：`polymath`。不要再安装已废弃的 `polymath-syllabus` / `polymath-coach` 分裂目录。

## 所有新对话都能用

把整个 `polymath` 目录复制到个人 Agent Store 的 `skills` 下面。目录名必须是 `polymath`，和 `SKILL.md` 里的 `name` 一致。斜杠命令 `/polymath` 来自这个名字；`syllabus` / `coach` 是同一命令下的模式词。

本机位置：

```text
~/Library/Application Support/Cursor/AgentStores/cursor_agent_stores/u480580782/files/skills/polymath
```

若仍存在旧的 `polymath-syllabus`、`polymath-coach`，删掉这两个目录，只保留 `polymath`。

复制之后**新开** Agent 对话。改了仓库源文件后再复制一次。

不要放进 `~/.cursor/skills-cursor/`。

## 装好的标志

新对话里输入 `/`，列表中有 `polymath`。可调用：

```text
/polymath syllabus
/polymath coach
```
