# Github 每日简报 Skill

一个将每日中文 GitHub AI 热门项目简报，按奥卡姆剃刀原则提炼成准确、简洁的 3:4 竖版科技封面文案与生图提示词的 Agent Skill。

## 文件结构

```text
github-daily-briefing-skill/
├── SKILL.md
├── references/
│   ├── design-rules.md
│   └── copywriting-rules.md
└── assets/
    └── image-prompt-template.md
```

## 安装

将 `github-daily-briefing-skill/` 整个目录复制到所用 Agent 支持的 skills 目录，并重新加载或重启 Agent。Codex 用户可将其放入 `$CODEX_HOME/skills/`，例如：

```text
$CODEX_HOME/skills/github-daily-briefing-skill/SKILL.md
```

## 每日使用

把当天的 GitHub AI 热门项目日报或候选项目列表发给 Agent，然后说：

> 使用 Github 每日简报 Skill，把今天的 GitHub AI 项目日报整理成一张 3:4 竖版封面文案和生图提示词。每次都自动按奥卡姆剃刀原则提炼，只保留必要且已核实的信息；请先核实项目与数据，无法核实的内容标出来，不要猜，并在结果中说明本次采用了奥卡姆剃刀。

也可以补充平台、日期、品牌色、Logo、图像生成工具，以及是否需要直接生成图片。默认交付包括事实核对表、精简后的封面文案和中文生图提示词。

## 输出原则

每次使用都必须应用奥卡姆剃刀：如无必要，勿增实体；只保留必要、准确、对读者有用的信息。项目名和数据以可追溯来源为准；无法确认时明确标注。每个项目只呈现一个核心价值，不把日报全文塞进图片。
