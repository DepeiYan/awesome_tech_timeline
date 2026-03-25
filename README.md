# ideaClaw 个人技术追踪助理 📚

> 让 AI 帮你管理技术知识，告别碎片化收藏

## 🎯 解决什么问题？

你是否也有这样的困扰：

- 看到好论文/项目 → 收藏 → **再也没有打开过**
- 微信/邮件里转发了一堆链接 → **找不到了**
- 浏览器书签堆积如山 → **不知道分类**
- 想跟进某个方向 → **忘记之前看过什么**

**ideaClaw + paper-tracker** 就是为此而生。

## ✨ 核心功能

### 一键追踪，自动整理

只需把链接发给 AI 助手，它会：

1. **访问链接** → 提取标题、作者、时间、核心贡献
2. **智能分类** → 自动判断技术领域（World Model、VLA/VLN、3D Reconstruction 等）
3. **生成笔记** → 创建详细笔记文件
4. **更新索引** → 维护分类目录和总索引
5. **同步仓库** → 自动 Git 提交和推送

### 支持多种来源

| 来源 | 示例 |
|------|------|
| arXiv 论文 | `https://arxiv.org/abs/2401.12345` |
| GitHub 项目 | `https://github.com/user/repo` |
| HuggingFace Papers | `https://huggingface.co/papers/2401.12345` |
| 技术博客 | 任意 URL |

### 技术领域自动归类

当前支持的领域分类：

- 🌍 **World Model** - 世界模型
- 🤖 **VLA/VLN** - 视觉语言动作/导航
- 🦾 **Embodied AI** - 具身智能
- 🎨 **3D Generation** - 3D 生成
- 🏗️ **3D Reconstruction** - 3D 重建
- 🎯 **Diffusion** - 扩散模型
- 💬 **LLM** - 大语言模型
- 👁️ **Vision** - 计算机视觉
- 🎮 **RL** - 强化学习

## 📁 输出结构

```
awesome_tech_timeline/
├── INDEX.md              # 总索引（按领域分表格）
├── world-model.md        # 世界模型领域
├── vla-vln.md            # VLA/VLN 领域
├── embodied-ai.md        # 具身智能领域
├── 3d-generation.md      # 3D 生成领域
├── 3d-reconstruction.md  # 3D 重建领域
├── papers/               # 论文详细笔记
│   ├── 2026-01-reli3d.md
│   └── 2026-03-fast-wam.md
├── projects/             # 项目详细笔记
└── [领域]/              # 各领域子目录
```

每篇笔记包含：

- 基本信息（标题、机构、作者、链接）
- 核心贡献（一句话概括）
- 技术方法（详细解读）
- 实验结果
- 局限性

## 🚀 使用方式

### 1. 获取 ideaClaw

- **Web**: [openclaw.ai](https://openclaw.ai)
- **移动端**: iOS/Android App
- **桌面端**: Windows/macOS/Linux

### 2. 配置 paper-tracker 技能

克隆模板仓库：

```bash
git clone https://github.com/yourname/awesome_tech_timeline.git
```

在 ideaClaw 工作区放置 `paper-tracker` 技能文件。

### 3. 开始使用

直接发送链接给 AI 助手：

```
用户: https://arxiv.org/abs/2401.12345

AI: ✅ 已追踪
    标题: XXX
    领域: World Model
    笔记: papers/2024-01-xxx.md
    已同步到 GitHub
```

## 💡 典型场景

### 场景 1: 通勤路上刷到好论文

微信收到推送 → 转发给 ideaClaw → 自动整理 → 回家后打开仓库深入阅读

### 场景 2: 组会讨论

同事提到一个方法 → 当场发链接给 ideaClaw → 讨论时随时调出笔记

### 场景 3: 文献调研

想了解某方向 → 打开 `INDEX.md` → 快速浏览已整理的所有论文 → 选择深入阅读

### 场景 4: 定期回顾

每周/每月打开仓库 → 按时间线回顾学过的内容 → 评估方向进展

## 🆚 对比其他方案

| 方案 | 问题 | ideaClaw |
|------|------|----------|
| 浏览器书签 | 不分类、不总结、不更新 | ✅ 自动分类、生成笔记 |
| 微信收藏 | 找不到、没结构 | ✅ 按领域组织、有索引 |
| Notion/Obsidian | 手动录入太麻烦 | ✅ 一键追踪、自动生成 |
| Zotero | 仅限论文、移动端不便 | ✅ 全平台、全类型支持 |
| GitHub Stars | 无结构、难检索 | ✅ 详细笔记、智能分类 |

## 📊 已追踪案例

| 项目 | 领域 | 简介 |
|------|------|------|
| ReLi3D | 3D 重建 | 稀疏视图可重光照 3D 重建，0.3 秒推理 |
| Fast-WAM | World Model | 跳过预测实现 4 倍加速 |
| Uni-Walker | Embodied AI | 首次定义终身具身导航学习 |
| CoSMo3D | 3D 生成 | LLM 引导的开放世界 3D 语义分割 |

[查看完整索引 →](INDEX.md)

## 🔗 相关链接

- **ideaClaw 官网**: [openclaw.ai](https://openclaw.ai)
- **技能市场**: [clawhub.com](https://clawhub.com)
- **社区**: [Discord](https://discord.com/invite/clawd)

---

> 💬 **一句话介绍**: 把链接发给 AI，它帮你整理成结构化的技术知识库。随时随地追踪，再也不会丢。