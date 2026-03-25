---
name: paper-tracker
description: 论文/技术项目追踪与管理技能。帮助用户追踪和整理技术论文、博客和项目，按技术领域分类归档。当用户发送论文链接、GitHub项目链接、博客链接请求追踪整理时触发。支持arXiv、GitHub、HuggingFace Papers等来源。触发关键词：追踪论文、记录论文、整理项目、paper tracker、技术笔记。
---

# Paper Tracker

追踪和整理技术论文、博客和项目，按技术领域分类归档。

> 💡 **使用方式**: 将此技能放入 ideaClaw 工作区的 `skills/paper-tracker/` 目录，即可通过 ideaClaw 随时随地追踪技术内容。

## 数据源支持

| 来源 | 链接特征 |
|------|----------|
| arXiv | `arxiv.org/abs/*` |
| GitHub | `github.com/*/*` |
| HuggingFace Papers | `huggingface.co/papers/*` |
| 博客 | 其他URL |

## 工作流程

### 1. 访问并分析链接内容

使用 `web_fetch` 工具访问链接，提取关键信息：

- **标题/名称**: 论文标题或项目名称
- **作者/机构**: 作者列表、所属机构
- **发布时间**: 发表日期
- **论文链接**: arXiv、DOI 等直接链接
- **代码仓库**: GitHub 等（如有）
- **核心贡献**: 一句话概括解决了什么问题、用什么方法、效果如何

### 2. 判断技术领域

根据内容判断所属技术领域，常见分类：

| 领域标识 | 领域名称 | 关键词 |
|----------|----------|--------|
| `world-model` | 世界模型 | World Model, World Action Model, WAM |
| `vla-vln` | VLA/VLN | Vision-Language-Action, VLN, 视觉语言导航 |
| `embodied-ai` | 具身智能 | Embodied, Robot Learning, 具身导航 |
| `3d-reconstruction` | 3D重建 | SLAM, NeRF, 3D Reconstruction, Gaussian Splatting |
| `3d-generation` | 3D生成 | 3D Generation, Text-to-3D, 3D Editing |
| `diffusion` | 扩散模型 | Diffusion, Image Generation, Video Generation |
| `llm` | 大语言模型 | LLM, GPT, Language Model, Transformer |
| `vision` | 计算机视觉 | Object Detection, Segmentation, CV |
| `rl` | 强化学习 | Reinforcement Learning, RL, Policy |

### 3. 创建详细笔记文件

在项目根目录下创建详细笔记文件：

```
awesome_tech_timeline/
├── papers/           # 论文详细笔记: YYYY-MM-title.md
├── projects/         # 项目详细笔记: project-name.md
├── 3d-reconstruction/ # 3D重建领域子目录
└── [其他领域]/       # 各领域子目录
```

笔记模板见 `templates/paper-note.md`。

### 4. 更新领域分类文件

找到或创建对应的领域分类文件 `[domain].md`，在表格中添加一行：

```markdown
| 名称 | 机构/来源 | 时间 | 简介 | 链接 |
|------|----------|------|------|------|
| [简短名称] | [机构] | [YYYY-MM] | [一句话简介] | [论文]() · [笔记]() |
```

简介格式：解决了什么问题，用什么方法，取得什么效果（控制在50字以内）

**⚠️ 排序规则**：表格按时间**从近到远**排序（最新的在最上面）

### 5. 更新 INDEX.md

更新总索引文件 `INDEX.md`，按技术领域划分为多个独立表格：

```markdown
### [领域名称] ([领域英文名])

| 名称 | 时间 | 简介 | 链接 |
|------|------|------|------|
| [项目名] | [时间] | [一句话简介] | [链接] |

[查看全部 →]([领域文件].md)
```

**⚠️ 排序规则**：
- 领域表格内按时间**从近到远**排序
- 时间线表格同样按时间**从近到远**排序

### 6. 提交变更

```bash
git add .
git commit -m "添加 [项目名称] 到 [领域]"
git push
```

## 目录结构

```
awesome_tech_timeline/
├── README.md              # 项目说明
├── INDEX.md               # 总索引（按领域分多个表格）
├── skills/                # 技能目录
│   └── paper-tracker/     # paper-tracker 技能
│       └── SKILL.md       # 技能定义文件
├── templates/             # 模板目录
│   └── paper-note.md      # 论文笔记模板
├── world-model.md         # 世界模型领域
├── vla-vln.md             # VLA/VLN 领域
├── embodied-ai.md         # 具身智能领域
├── 3d-generation.md       # 3D生成领域
├── 3d-reconstruction.md   # 3D重建领域
├── [其他领域].md          # 其他技术领域
├── papers/                # 论文详细笔记
├── projects/              # 工具/项目
└── [领域]/                # 各领域子目录
```

## 使用示例

```
用户: 追踪这篇论文 https://arxiv.org/abs/2401.12345

助手: 
1. 访问链接提取信息
2. 判断领域（如：world-model）
3. 创建 papers/2024-01-paper-title.md
4. 更新 world-model.md
5. 更新 INDEX.md
6. git commit & push
```

## 简介撰写要求

- 控制在 50 字以内
- 格式：解决了什么问题，用什么方法，取得什么效果
- 示例：
  - "无需训练的长时序3D重建方法，解决漂移与退化问题，误差降低40%"
  - "首次定义终身具身导航学习，提出DE-LoRA架构，遗忘率降低70%"

## 关键原则

1. **按技术领域分类**，不按文档类型分类
2. **INDEX.md 按领域分多个表格**，每个领域一个独立表格
3. **简介要简洁**：一句话说清楚问题、方法、效果
4. **链接要完整**：论文、代码、原文都要记录
5. **保持同步**：详细笔记、领域分类、总索引三者一致

## 快速开始

1. 克隆项目：
   ```bash
   git clone https://github.com/yourname/awesome_tech_timeline.git
   ```

2. 将 `skills/paper-tracker/` 目录复制到你的 ideaClaw 工作区

3. 开始追踪：直接向 ideaClaw 发送链接即可

## 参考资料

- 详细领域分类指南：`references/domain-guide.md`
- 笔记模板：`templates/paper-note.md`