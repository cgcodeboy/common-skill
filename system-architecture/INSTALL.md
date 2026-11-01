# 安装

源文件是本目录。仓库里的这一份是改动的依据。Cursor 不会因为仓库里有这个文件夹，就在其他项目的新对话里自动启用它。

## 所有新对话都能用

把整个 `system-architecture` 目录复制到个人 Agent Store 的 `skills` 下面。目录名必须是 `system-architecture`，和 `SKILL.md` 里的 `name` 一致。斜杠命令 `/system-architecture` 来自这个名字。

本机已经验证过的位置是：

```text
~/Library/Application Support/Cursor/AgentStores/cursor_agent_stores/u480580782/files/skills/system-architecture
```

复制时覆盖该目录下的文件，不要多包一层文件夹。复制之后新开一个 Agent 对话，输入 `/system-architecture`。当前已经打开的对话不会重新加载技能列表。

改了仓库里的源文件之后，再复制一次。两处不会自动同步。

不要放进 `~/.cursor/skills-cursor/`。那是 Cursor 自己的技能目录。

## 只在某一个仓库里用

若只想让某个产品仓库的协作者使用，把本目录放到那个仓库的 `.cursor/skills/system-architecture/`。这样它只在那个仓库里出现。本仓库不采用这种方式：common-skill 的每个技能就是根目录下的一个文件夹。

## 装好的标志

新对话里输入 `/`，列表中有 `system-architecture`。不输入斜杠、只讨论系统架构、选型、C4、4+1 或架构评审时，对话也会按技能描述判断要不要使用它。技能没有把自动调用关掉。
