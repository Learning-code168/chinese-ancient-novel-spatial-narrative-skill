# 中国古代小说空间叙事论文格式 Skill

适用于中国古代小说空间叙事研究课程论文的 Codex Skill。它帮助在保留作者正文内容的前提下，统一 Word 论文的标题、摘要、章节、正文、原著引文、脚注和参考文献格式，并在交付前检查排版。

本技能特别适用于要求按「中国古代小说空间叙事研究」课程论文规范排版的 `.docx` 文件；内容包括中文标点、原著引文段落、《红楼梦》引文页码脚注、脚注编号以及中外文参考文献排序等。

> **适用范围：仅适用于汕头大学汉语言文学专业 2024 级的课程论文作业。**其他年级、专业或用途的论文，请先确认其课程要求，不要默认套用本规范。

## 安装

将仓库克隆到 Codex 的个人技能目录：

```powershell
git clone https://github.com/Learning-code168/chinese-ancient-novel-spatial-narrative-skill.git `
  "$env:USERPROFILE\.codex\skills\zhongguo-gudai-kongjian-xushi-lunwen-geshi"
```

若使用 `CODEX_HOME` 指定了其他 Codex 数据目录，请将仓库克隆到该目录下的 `skills/zhongguo-gudai-kongjian-xushi-lunwen-geshi`。安装后，在 Codex 中请求创建、检查或格式化相关论文即可触发该技能；也可以显式调用 `$zhongguo-gudai-kongjian-xushi-lunwen-geshi`。

## 文件

- `SKILL.md`：技能说明、Word 格式规则、脚注与参考文献规范及交付前检查项。
- `agents/openai.yaml`：Codex 中显示的技能名称、简介和默认提示。

## 作者与许可证

作者：[@Learning-code168](https://github.com/Learning-code168)。

本仓库使用 [MIT License](LICENSE)。

---

# Chinese Ancient Fiction Spatial Narrative Formatting Skill

A Codex Skill for formatting Word course papers about spatial narrative in ancient Chinese fiction. It helps preserve the author's writing while applying consistent title, abstract, heading, body-text, quotation, footnote, and bibliography styles.

The guidance is tailored to the “中国古代小说空间叙事研究” course-paper format. It covers Chinese punctuation, classical-text quotation blocks, page citations for quotations from *Dream of the Red Chamber*, footnote numbering, and reference ordering.

> **Scope: This Skill applies only to course-paper assignments for the 2024 cohort of the Chinese Language and Literature major at Shantou University.** Do not assume it applies to other cohorts, majors, or purposes without first confirming their course requirements.

## Install

Clone this repository into your personal Codex skills directory:

```powershell
git clone https://github.com/Learning-code168/chinese-ancient-novel-spatial-narrative-skill.git `
  "$env:USERPROFILE\.codex\skills\zhongguo-gudai-kongjian-xushi-lunwen-geshi"
```

If you use a custom `CODEX_HOME`, clone it into `skills/zhongguo-gudai-kongjian-xushi-lunwen-geshi` under that directory. Then ask Codex to create, check, or format a relevant paper, or invoke `$zhongguo-gudai-kongjian-xushi-lunwen-geshi` explicitly.

## Author and license

Author: [@Learning-code168](https://github.com/Learning-code168).

Licensed under the [MIT License](LICENSE).
