# Doctoral Dissertation Skills

面向博士大论文写作、整合、结构重构、证据审计、语言优化与最终定稿的模块化 Agent Skills。

[![skills.sh](https://skills.sh/b/syc9336-rgb/doctoral-dissertation-skills)](https://skills.sh/syc9336-rgb/doctoral-dissertation-skills)
[![Latest Release](https://img.shields.io/github/v/release/syc9336-rgb/doctoral-dissertation-skills?display_name=tag&sort=semver)](https://github.com/syc9336-rgb/doctoral-dissertation-skills/releases/latest)
[![Apache-2.0](https://img.shields.io/github/license/syc9336-rgb/doctoral-dissertation-skills)](LICENSE)

> 不是替你虚构论文内容，而是把真实研究材料组织成可审计、可重构、可定稿的博士论文工作流。

## 先试用

安装后，在 Codex、Claude Code 或其他支持 Agent Skills 的工具中输入：

```text
使用 doctoral-dissertation skill。
先读取当前项目真实材料，建立 Frozen Facts Table、
Claim–Evidence Matrix 和 RQ Closure Matrix。
不要继承上一项目的案例、样本、变量或研究结构，
再根据真实证据重建博士论文结构。
```

## 一条命令安装

```bash
npx skills add syc9336-rgb/doctoral-dissertation-skills \
  --skill doctoral-dissertation --yes --copy
```

当前包含：

- `doctoral-dissertation`：博士大论文全流程写作、结构、语言、证据与定稿 Skill。

本项目采用 **Apache License 2.0** 开源发布。你可以在许可证条款范围内使用、复制、修改、fork、再发布、集成及商业使用。

## 为什么做这个 Skill

博士论文的核心问题通常不是“缺少字数”，而是：

- 研究事实与论文叙述不一致；
- 旧目录绑架真实研究；
- 小论文被机械拼接；
- 章节没有独立功能；
- 文献综述变成作者列队；
- 方法、结果、讨论彼此混写；
- 正文出现大量过程性、推导性和防御性语言；
- 为了严谨而过度克制，削弱本应明确表达的理论价值；
- 图表、附录、脚注和多语言版本缺少系统审计。

`doctoral-dissertation` Skill 将这些问题组织为一套可复用工作流。

## 仓库结构

```text
doctoral-dissertation-skills/
├── LICENSE
├── NOTICE
├── README.md
├── README_EN.md
├── CONTRIBUTING.md
├── CHANGELOG.md
├── CITATION.cff
└── skills/
    └── doctoral-dissertation/
        ├── SKILL.md
        ├── README.md
        ├── README_EN.md
        ├── tasks/
        ├── references/
        └── examples/
```

`skills/` 下每个顶层目录都是一个独立 Skill 单元，便于后续继续扩展。

## 安装

### 使用 `npx skills`

查看可安装 Skill：

```bash
npx skills add syc9336-rgb/doctoral-dissertation-skills --list
```

安装 `doctoral-dissertation`：

```bash
npx skills add syc9336-rgb/doctoral-dissertation-skills \
  --skill doctoral-dissertation --yes --copy
```

全局安装到 Codex：

```bash
npx skills add syc9336-rgb/doctoral-dissertation-skills \
  --global --agent codex --skill doctoral-dissertation --yes --copy
```

### 手动安装到 Codex

```bash
git clone https://github.com/syc9336-rgb/doctoral-dissertation-skills.git
mkdir -p ~/.codex/skills
cp -R doctoral-dissertation-skills/skills/doctoral-dissertation ~/.codex/skills/
```

请复制完整 Skill 目录，而不是只复制 `SKILL.md`，因为该 Skill 还依赖 `tasks/`、`references/` 和 `examples/`。

## 使用示例

```text
使用 doctoral-dissertation skill。
先读取当前项目真实材料，建立 Frozen Facts Table、
Claim–Evidence Matrix 和 RQ Closure Matrix。
不要继承上一项目的任何案例、样本、变量或研究结构，
再根据真实证据重建整篇博士论文。
```

或：

```text
使用 doctoral-dissertation skill 重写这一章。
正文采用完成态学术表达，删除过程性、推导性、提前防御和散落式局限句；
证据充分的地方不要因为过度克制而削弱理论判断。
```

## 适合哪些任务

- 从真实材料重建博士论文总体结构；
- 重构章节、节和段落的功能边界；
- 建立研究问题、证据和核心论断之间的闭环；
- 组织文献综述、理论框架与研究设计；
- 分离并整合方法、结果与讨论；
- 审计图表、附录、脚注、引用和多语言版本；
- 在答辩或提交前执行完整性与一致性检查。

## 贡献与反馈

欢迎通过 [Issues](https://github.com/syc9336-rgb/doctoral-dissertation-skills/issues)、
[Discussions](https://github.com/syc9336-rgb/doctoral-dissertation-skills/discussions)
和 Pull Request 提交问题、脱敏案例与改进建议。

反馈时请尽量说明：使用的任务、输入材料类型、期望结果、实际结果，以及是否可以公开复现。

## 核心原则

- 真实性高于目录完整性；
- 原始证据高于后期叙述；
- 章解决大问题，节解决子问题，小节形成核心判断；
- 正文呈现研究完成态，而不是作者思考或修改过程；
- 不预设结果；
- 不为“严谨”习惯性降低所有结论强度；
- 局限集中处理；
- 每项核心结论必须有证据锚点；
- 重大修改必须执行全文连锁影响扫描。

## 贡献

欢迎 Issue、Pull Request、fork 和衍生开发。详见 [CONTRIBUTING.md](CONTRIBUTING.md)。

## License

Apache License 2.0。详见 [LICENSE](LICENSE) 和 [NOTICE](NOTICE)。

