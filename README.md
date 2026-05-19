# viral-title-breakdown

爆款标题拆解 Skill：先根据用户方向生成业务定位，再拆解标题为什么会爆，并改写成适合用户自己业务的新标题。

## 一键安装

### Claude Code

```bash
npx skills add sungwong/viral-title-breakdown --skill viral-title-breakdown --agent claude-code -g -y
```

### Codex

```bash
npx skills add sungwong/viral-title-breakdown --skill viral-title-breakdown --agent codex -g -y
```

### OpenClaw

```bash
npx skills add sungwong/viral-title-breakdown --skill viral-title-breakdown --agent openclaw -g -y
```

## 使用

安装后直接说：

```text
帮我拆标题
```

如果你还没有清晰定位，它会先让你用自然语言说一说方向，再帮你生成并校准《业务定位卡》。

## 可选：写入飞书表格

这个 Skill 默认只在对话里输出拆解结果，**不会自动写入任何飞书表格**。

如果你希望把拆解结果追加到自己的飞书表格，需要额外满足：

1. 你的 AI 环境已安装并配置飞书 / Lark 表格相关能力，例如 `lark-sheets`、飞书表格 Skill 或飞书连接器。
2. 你提供自己的飞书表格链接或 token。
3. 你确认要写入的字段结构。

推荐表头：

```text
原标题｜选题｜人群｜痛点｜反常识观点｜情绪｜传播点｜钩子公式｜改写-贴图版｜改写-长文版
```

注意：Skill 不会、也不应该写入作者的飞书表格。每个用户都需要连接自己的飞书账号，并提供自己的目标表格。
