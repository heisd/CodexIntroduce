# Codex 使用笔记与主题导航

整理 Codex 使用过程中关于任务协作、上下文、权限、初始化与代码审查的个人学习笔记。正文分布在各 Markdown 文件中，本页说明阅读顺序与主题关联。

这些内容属于写作时的经验记录，部分文件标题使用命令名。本文导航不构成对当前所有版本、平台或界面均支持这些命令的保证。

## 快速阅读路线

| 目的 | 建议顺序 |
| --- | --- |
| 第一次整理项目工作方式 | 初始化 → 引用文件 → 权限 |
| 长任务上下文管理 | compact → fork |
| 理解任务协作 | agent → agent 与 subagents → collab |
| 检查代码改动 | diff 与 review → review 场景 |
| 调整使用体验 | personality → experimental |
| 了解停止与进程 | ps/stop |

## 全部文档

| 文件 | 阅读内容 |
| --- | --- |
| [init-intro.md](./init-intro.md) | 初始化相关笔记 |
| [mention-intro.md](./mention-intro.md) | 引用与上下文材料 |
| [permissions-intro.md](./permissions-intro.md) | 权限类型、配置关系与使用建议 |
| [compact-intro.md](./compact-intro.md) | 长会话中的上下文压缩与使用时机 |
| [fork-intro.md](./fork-intro.md) | 分叉讨论与使用场景 |
| [agent-intro.md](./agent-intro.md) | Agent、角色分工与工作流 |
| [agent-vs-subagents-intro.md](./agent-vs-subagents-intro.md) | Agent 与子任务协作方式的比较 |
| [collab-intro.md](./collab-intro.md) | 协作方式与使用场景 |
| [diff-review-code-audit.md](./diff-review-code-audit.md) | 变更查看与代码审查的配合 |
| [review-use-cases.md](./review-use-cases.md) | 审查场景 |
| [personality-intro.md](./personality-intro.md) | 表达风格相关笔记 |
| [experimental-intro.md](./experimental-intro.md) | 实验功能记录 |
| [ps-stop-intro.md](./ps-stop-intro.md) | 运行状态与停止相关笔记 |

## 本地阅读

```bash
git clone --branch Macmini https://github.com/heisd/CodexIntroduce.git
cd CodexIntroduce
```

使用 Markdown 阅读器或直接在 GitHub 中打开文件即可，没有应用依赖和构建步骤。默认分支名为 `Macmini`，这是仓库现有分支名称。

## 如何使用这些笔记

先按具体目的选择主题，再对照自己安装的版本、当前可见功能和实际配置。遇到正文中出现但界面中不存在的命令，应检查适用版本与平台，不必仅为匹配笔记修改本机设置。

笔记中的“建议工作流”是经验总结，应结合项目规模、团队协作和当前任务调整。尤其是协作与审查主题，应关注输入材料、任务边界与结果验证，而不是只复制一个命令名。

## 后续维护约定

补充或修正笔记时，建议同时记录适用平台、写作日期、版本线索、实际使用入口与可核对的例子；将观察到的行为与个人建议分开，以便后续更新。一个主题保留一份主体文档，本页维护索引，减少内容重复和版本不一致。
