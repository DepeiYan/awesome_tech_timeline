# Tech Notes - 技术追踪

> 按技术领域分类的技术项目追踪，记录最新的论文、工具和博客

**创建时间:** 2026-03-24  
**维护者:** LittleBrother 🤖

---

## 📁 目录结构

```
tech-notes/
├── README.md              # 本说明文件
├── INDEX.md               # 总索引（主文档）
├── world-model.md         # 世界模型领域
├── embodied-ai.md         # 具身智能领域
├── 3d-reconstruction.md   # 3D重建领域
├── papers/                # 论文详细笔记
│   └── YYYY-MM-title.md
├── projects/              # 工具/项目
│   └── project-name.md
└── 3d-reconstruction/     # 3D重建相关笔记
    └── YYYY-MM-title.md
```

---

## 🏷️ 技术领域

| 领域 | 文件 | 描述 |
|------|------|------|
| **World Model** | [world-model.md](./world-model.md) | 世界模型、VLA大模型、机器人 |
| **Embodied AI** | [embodied-ai.md](./embodied-ai.md) | 具身智能、具身导航、VLN |
| **3D Reconstruction** | [3d-reconstruction.md](./3d-reconstruction.md) | 3D重建、SLAM、NeRF |

---

## 🤖 自动整理规则

当你发送链接给我时，我会：

1. **自动判断技术领域**
   - 世界模型 (World Model)
   - 具身智能 (Embodied AI)
   - 3D重建 (3D Reconstruction)
   - 其他新兴领域

2. **提取关键信息**
   - 标题、作者、机构
   - 发表时间、来源
   - 核心贡献/要点
   - 论文/代码链接

3. **归档到对应领域**
   - 创建详细笔记文件
   - 更新领域分类文件
   - 更新 INDEX.md 索引

4. **Git 提交**
   - 自动 commit 变更
   - 清晰的提交信息

---

## 🚀 使用方式

直接发送链接给我，例如：
- "看看这个 https://arxiv.org/abs/xxxx.xxxxx"
- "记录这篇博客 https://xxx.com/blog/xxx"
- "这个项目不错 https://github.com/xxx/xxx"