# Meta-Circle Strategy

用于研究与战略工作的可复用 Codex 技能。

## 论文翻译技能

| 技能 | 调用名称 | 内容 |
| --- | --- | --- |
| [论文完整翻译](skills/paper-full-translation/SKILL.md) | `$paper-full-translation` | 逐段翻译全文、附录、图表文字及参考文献题名，提供可批注离线阅读器、快速阅读与教程式导读。 |
| [论文简要翻译](skills/paper-brief-translation/SKILL.md) | `$paper-brief-translation` | 完整翻译摘要、序言／引言、总结／结论，提供逐段中英对照、可批注离线阅读器和教程式导读。 |

简要翻译缩小的是章节范围，所选章节仍然逐段完整翻译。

## 论文解读技能

| 技能 | 调用名称 | 内容 |
| --- | --- | --- |
| [论文解读小红书版本](skills/paper-reading-xiaohongshu/SKILL.md) | `$paper-reading-xiaohongshu` | 围绕切入点制作机制图解、实验结果与领域缺口分析，交付图卡、同步发布文案、预览和来源说明。 |
| [论文解读公众号版本](skills/paper-reading-wechat/SKILL.md) | `$paper-reading-wechat` | 参考个人原创分析风格，默认约2000—2500字，解读论文图表与研究洞察，交付可编辑Word。 |

解读任务可以直接使用论文或已有译文。只要求要点时提供提纲；要求完整内容时生成对应发布材料。研究关联按主题需要加入。

## 事件推广方案技能

| 技能 | 调用名称 | 内容 |
| --- | --- | --- |
| [事件推广方案制作Skill](skills/event-promotion-plan/SKILL.md) | `$event-promotion-plan` | 梳理核心内容、受众、渠道分工、传播指标与发布时间，按需制作可编辑 PPT 和执行文档，并跟进复盘。 |

包含[两页成果发布方案示例](skills/event-promotion-plan/references/two-slide-launch-example.md)，说明原始材料核对、两页 PPT 的结构和修改要点，供团队按具体事件复用。

## 安装

将 `skills/` 下需要的技能文件夹复制到个人 Codex 技能目录 `~/.codex/skills/`，保留各文件夹内的 `SKILL.md`、`agents/` 和 `references/`。

## 使用

提供论文文件或链接，输入：

```text
使用 $paper-full-translation 翻译这篇论文：[文件或链接]
```

或：

```text
使用 $paper-brief-translation 翻译这篇论文：[文件或链接]
```

每篇论文默认使用“序号＋论文标题”独立文件夹，英文原文与中文译文上下对照，并附教学导读与支持高亮、划线、笔记、备份恢复的离线阅读器。具体任务中指定的范围与格式优先。

解读论文时，输入：

```text
使用 $paper-reading-xiaohongshu 解读这篇论文：[文件或链接]，切入点是：[问题或角度]
```

或：

```text
使用 $paper-reading-wechat 将这篇论文写成公众号解读：[文件或链接]，参考我的原创文章风格
```

制作事件推广方案时，输入：

```text
使用 $event-promotion-plan 根据这些研究材料制作两页成果发布方案，面向全球 AI 研究员，明确内容、渠道、预期结果和关键时间线：[材料]
```

## 目录

```text
skills/
├── paper-full-translation/
│   ├── SKILL.md
│   ├── agents/openai.yaml
│   └── references/reading-package.md
├── paper-brief-translation/
│   ├── SKILL.md
│   ├── agents/openai.yaml
│   └── references/reading-package.md
├── paper-reading-xiaohongshu/
│   ├── SKILL.md
│   ├── agents/openai.yaml
│   └── references/research-checks.md
├── paper-reading-wechat/
│   ├── SKILL.md
│   ├── agents/openai.yaml
│   └── references/research-checks.md
└── event-promotion-plan/
    ├── SKILL.md
    ├── agents/openai.yaml
    └── references/two-slide-launch-example.md
```
