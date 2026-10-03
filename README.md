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

### ui-design

将二十条 UI 设计原则转成页面与组件设计、优化和视觉审查中的具体决策：先建立灰度层级，再处理留白、排版、色阶、图片与空状态。

复用已有品牌和设计系统，按内容与设备调整参数；参考规则同时说明适用边界，避免机械套用数值。

## 示例

[项目工作台](examples/ui-design/)：包含桌面表格、移动端列表与表格切换，以及搜索、筛选、新建、导出和批量删除。下载后可直接打开 HTML。

## 安装

```bash
npx skills add leowux/skills
```

安装过程中选择 `show-me` 或 `ui-design`，并按提示安装到目标 Agent。

## 使用

```text
$show-me
$show-me markdown table
$show-me mermaid
$show-me html
$ui-design 设计一个项目管理页面
$ui-design 优化当前页面的层级和留白
$ui-design 审查这张截图的视觉问题
```

`show-me` 没有参数时可视化当前对话主题；提供格式参数时优先使用指定格式。`ui-design` 使用当前相关界面，按请求设计、修改或审查。

## 目录

```text
skills/
├── show-me/
│   └── SKILL.md
└── ui-design/
    ├── SKILL.md
    ├── agents/
    │   └── openai.yaml
    └── references/
        └── design-rules.md
```

## License

[MIT](LICENSE)
