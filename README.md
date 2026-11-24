# Meta-Circle Strategy

用于研究与战略工作的可复用 Codex 技能。

## 论文翻译技能

| 技能 | 调用名称 | 内容 |
| --- | --- | --- |
| [论文完整翻译](skills/paper-full-translation/SKILL.md) | `$paper-full-translation` | 逐段翻译全文、附录、图表文字及参考文献题名，提供可批注离线阅读器、快速阅读与教程式导读。 |
| [论文简要翻译](skills/paper-brief-translation/SKILL.md) | `$paper-brief-translation` | 完整翻译摘要、序言／引言、总结／结论，提供逐段中英对照、可批注离线阅读器和教程式导读。 |

简要翻译缩小的是章节范围，所选章节仍然逐段完整翻译。

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

## 目录

```text
skills/
├── paper-full-translation/
│   ├── SKILL.md
│   ├── agents/openai.yaml
│   └── references/reading-package.md
└── paper-brief-translation/
    ├── SKILL.md
    ├── agents/openai.yaml
    └── references/reading-package.md
```
