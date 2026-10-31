# Scientific Paper Workflow · 科研论文撰写 Skill

一个以文献与实验依据为核心的科研写作技能。支持分节撰写、局部修改、翻译、文献核查、图表解释和科学性审阅。

## 核心工作方式

- 围绕当前小节检索与阅读相关文献，避免无关旧稿影响当前内容。
- 区分“行文逻辑参考”和“科学内容依据”，记录来源与原文位置。
- 区分实测数据、拟合结果、模型预测和机理解释，不虚构缺失结果。
- 按指定范围修改；仅审阅时提供问题与建议，不自动重写全文。
- 根据使用者的领域、期刊和输出语言适配，不内置任何个人论文结论。

## 下载和安装

在 GitHub 仓库页面选择 **Code → Download ZIP**，解压后取得 `sci-paper-workflow` 文件夹。

推荐按项目安装：将该文件夹放到项目的 `.agents/skills/` 中，最终结构如下：

```text
your-project/
└── .agents/
    └── skills/
        └── sci-paper-workflow/
            ├── SKILL.md
            ├── agents/openai.yaml
            └── references/
                ├── writing.md
                ├── literature.md
                ├── figure-data.md
                ├── review.md
                └── evidence-records.md
```

这是一个技能，五份 reference 是按需读取的内部模块，不需要分别安装。不要只复制 SKILL.md。若同名目录已存在，请先备份，避免覆盖自己的修改。

在 Codex 中打开该项目，并在新的消息中使用 `$sci-paper-workflow`。其他支持 Agent Skills 的工具可按各自安装方式使用此目录；本发布包未逐一验证其他工具。

安装目录依据：[OpenAI 官方技能文档](https://learn.chatgpt.com/docs/build-skills)。

## 使用示例

```text
使用 $sci-paper-workflow，根据我提供的数据撰写这一小节。
先检索相关文献并核查原文，再组织段落。
输出英文稿、中文翻译，以及实际引用文献和对应依据。
```

```text
使用 $sci-paper-workflow，只修改下面段落的语言表达，
保留观点、数据、引用和结构，不扩写其他内容。
```

```text
使用 $sci-paper-workflow，检查这段讨论的科学依据和引用是否匹配。
先给出有位置和证据的问题，不直接改写正文。
```

可在请求中提供研究领域、目标期刊、当前小节任务和语言要求。长期偏好可放在自己项目的说明文件中，实际数据与证据记录仍留在自己的项目内。未指定时使用相关领域的同行评议原始研究；默认正文语言为英文，中译按需求提供。

## 文件与访问边界

本包只提供通用工作流，不包含论文正文、文献 PDF、实验/训练数据、模型权重、逐点预测、证据记录实例、个人目录或凭据。

包内没有可执行脚本、自动上传程序或额外服务配置。检索与文件阅读依赖使用者所用工具的现有能力及授权；它不提供付费论文访问权限，也不能代替研究者核实结果。无法获取全文时应明确标注核查范围。

使用者的论文、数据和私人文献索引不应保存到技能目录或提交到此仓库。复用这些流程并不授权对外分享研究材料。

## English overview

A portable Agent Skill for evidence-led scientific manuscript drafting, targeted revision, translation, literature verification, figure interpretation, and scientific review. Install the complete `sci-paper-workflow` directory under your project's `.agents/skills/`, then invoke `$sci-paper-workflow`. Research data and project-specific evidence belong in your own project, outside this reusable package.
