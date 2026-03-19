# Codex `/experimental` 与实验功能说明（Mac）

在 Codex CLI 里，`/experimental` 可以理解为“实验功能入口”。  
它用于查看、启用、禁用尚在试验阶段的能力。

## 1. 核心概念

- 实验功能通常还在迭代，行为和参数可能变化。
- 开启后可能带来新能力，也可能有稳定性风险。
- 适合先小范围试用，再决定是否长期启用。

## 2. 你当前版本的对应用法

你这台机器上，主要通过 `codex features` 来管理实验功能：

```bash
codex features list
codex features enable <feature_name>
codex features disable <feature_name>
```

也可以只在当前启动时临时切换：

```bash
codex --enable <feature_name>
codex --disable <feature_name>
```

## 3. 推荐使用流程

1. 先执行 `codex features list` 查看功能名、阶段和当前状态。
2. 先用临时开关试跑一两个会话（`--enable`）。
3. 验证稳定后，再使用 `codex features enable` 做全局启用。
4. 出现问题时，立即 `disable` 回退。

## 4. 配置范围说明

- `codex features enable/disable`：通常写入 `~/.codex/config.toml`，对后续会话生效。
- `--enable/--disable`：只影响当前这次命令启动的会话。

## 5. 实战建议

- 不要一次开启太多实验项，便于定位问题来源。
- 变更前后记录一次 `features list` 输出，方便回滚。
- 生产任务优先使用稳定功能，实验功能用于验证和探索。
