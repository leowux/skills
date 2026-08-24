# Agent Skills

[![skills.sh](https://skills.sh/b/leowux/skills)](https://skills.sh/leowux/skills)

一个面向 Codex、Claude Code 等兼容 Agent Skills 的个人技能仓库。

## 包含的技能

### show-me

根据当前主题选择最小且有用的视觉表达：

- Markdown 表格：比较、映射、矩阵和结构化事实
- Mermaid：流程、时序、状态、架构和数据关系
- 自包含 HTML：自定义布局、交互模拟和复杂 UI 状态

显式指定主题或格式时优先遵从；没有参数时使用最近且最相关的对话上下文。

## 安装

```bash
npx skills add leowux/skills
```

安装过程中选择 `show-me`，并按提示安装到目标 Agent。

## 使用

```text
$show-me
$show-me markdown table
$show-me mermaid
$show-me html
```

没有参数时，技能会直接可视化当前对话主题；提供格式参数时，则优先使用指定格式。

## 目录

```text
skills/
└── show-me/
    └── SKILL.md
```

## License

[MIT](LICENSE)
