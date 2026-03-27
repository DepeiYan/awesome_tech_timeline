# 技术备忘索引 - Tech Notes Index

> 所有技术文档的总索引

**创建时间:** 2026-03-24  
**最后更新:** 2026-03-25

---

## 📂 按技术领域分类

### Vision / Geospatial (视觉与地理空间)

| 名称 | 时间 | 简介 | 链接 |
|------|------|------|------|
| TerraScope | 2026-03 | 首个像素级地理空间推理 VLM，支持多模态灵活推理与多时序变化分析，性能远超 GPT-4o | [arXiv](https://arxiv.org/abs/2603.19039) · [笔记](papers/2026-CVPR-terrascope.md) |

[查看全部 →](vision-geospatial.md)

---

### World Model (世界模型)

| 名称 | 时间 | 简介 | 链接 |
|------|------|------|------|
| Fast-WAM | 2026-03 | 质疑 WAM 推理时未来想象的必要性，跳过预测实现 4 倍加速且性能相当 | [论文](https://arxiv.org/abs/2603.16666) · [笔记](papers/2026-03-fast-wam.md) |

[查看全部 →](world-model.md)

---

### VLA/VLN (视觉语言动作/导航)

| 名称 | 时间 | 简介 | 链接 |
|------|------|------|------|
| Towards Generalist Embodied AI: A Survey on World Models for VLA Agents | 2026-03 | 首篇 VLA 与世界模型交叉领域综述，提出四大范式分类法 | [论文](https://doi.org/10.36227/techrxiv.176948355.54623875/v1) · [笔记](papers/2026-03-vla-world-models-survey.md) |
| awesome-world-models-for-vla-agents | 2026-03 | VLA 世界模型领域论文汇总，含 CALVIN/LIBERO 排行榜 | [GitHub](https://github.com/FutureTwT/awesome-world-models-for-vla-agents) · [笔记](projects/awesome-world-models-for-vla-agents.md) |
| 3D Gaussian Map for VLN | 2025 | 结合 3D Gaussian Splatting 与开放集语义分组的视觉语言导航方法 | [论文](https://openaccess.thecvf.com/content/ICCV2025/papers/Gao_3D_Gaussian_Map_with_Open-Set_Semantic_Grouping_for_Vision-Language_Navigation_ICCV_2025_paper.pdf) · [笔记](papers/2025-ICCV-3d-gaussian-map-vln.md) |

[查看全部 →](vla-vln.md)

---

### Embodied AI (具身智能)

| 名称 | 时间 | 简介 | 链接 |
|------|------|------|------|
| Uni-Walker (Lifelong Embodied Navigation Learning) | 2026-03 | 首次定义终身具身导航学习(LENL)，提出 DE-LoRA 架构解决灾难性遗忘，遗忘率降低 70% | [论文](https://arxiv.org/abs/2603.06073) · [笔记](papers/2026-03-uni-walker-lenl.md) |

[查看全部 →](embodied-ai.md)

---

### 3D Generation (3D生成)

| 名称 | 时间 | 简介 | 链接 |
|------|------|------|------|
| Hi-GRPO | 2026 | 首个系统性研究 RL 用于 3D 生成，提出层次化方法开创新路径 | [公众号](https://mp.weixin.qq.com/s/fJ1FkFhZJ5c0tl3fGLj-Xw) · [笔记](papers/2026-CVPR-hi-grpo.md) |
| CoSMo3D | 2026-03 | 通过 LLM 引导的规范空间建模，实现开放世界可提示的 3D 语义部件分割 SOTA | [论文](https://arxiv.org/abs/2603.01205) · [笔记](papers/2026-03-cosmo3d.md) |

[查看全部 →](3d-generation.md)

---

### 3D Reconstruction (3D重建)

| 名称 | 时间 | 简介 | 链接 |
|------|------|------|------|
| MeMix | 2026-03 | 无需训练的长时序 3D 重建方法，解决漂移与退化问题，误差降低 40% | [博客](https://mp.weixin.qq.com/s/pV6D4jpBywQhWbxp8iK50A) · [笔记](3d-reconstruction/2026-03-memix-3d-reconstruction.md) |
| ReLi3D | 2026-01 | 稀疏视图可重光照 3D 重建，一次性解耦材质与光照，0.3 秒推理 | [主页](https://reli3d.jdihlmann.com/) · [笔记](papers/2026-01-reli3d.md) |
| BuildingWorld | 2025-11 | 500万 LOD2 建筑数据集，覆盖全球多样风格，支持城市基础模型训练 | [论文](https://arxiv.org/abs/2511.06337) · [笔记](papers/2025-11-buildingworld.md) |

[查看全部 →](3d-reconstruction.md)

---

## 📅 按时间线排序

| 时间 | 项目/论文 | 领域 | 链接 |
|------|----------|------|------|
| 2026-03 | TerraScope: 像素级地理空间推理 VLM | Vision / Geospatial | [arXiv](https://arxiv.org/abs/2603.19039) · [笔记](papers/2026-CVPR-terrascope.md) |
| 2026 | Hi-GRPO: RL 用于 3D 生成 | 3D Generation | [公众号](https://mp.weixin.qq.com/s/fJ1FkFhZJ5c0tl3fGLj-Xw) · [笔记](papers/2026-CVPR-hi-grpo.md) |
| 2026-03 | Fast-WAM: 世界动作模型推理优化 | World Model | [论文](https://arxiv.org/abs/2603.16666) · [笔记](papers/2026-03-fast-wam.md) |
| 2026-03 | Uni-Walker: 终身具身导航学习 | Embodied AI | [论文](https://arxiv.org/abs/2603.06073) · [笔记](papers/2026-03-uni-walker-lenl.md) |
| 2026-03 | VLA 世界模型综述 | VLA/VLN | [论文](https://doi.org/10.36227/techrxiv.176948355.54623875/v1) · [笔记](papers/2026-03-vla-world-models-survey.md) |
| 2026-03 | MeMix: 长时序 3D 重建方法 | 3D Reconstruction | [博客](https://mp.weixin.qq.com/s/pV6D4jpBywQhWbxp8iK50A) · [笔记](3d-reconstruction/2026-03-memix-3d-reconstruction.md) |
| 2026-03 | CoSMo3D: 开放世界 3D 语义部件分割 | 3D Generation | [论文](https://arxiv.org/abs/2603.01205) · [笔记](papers/2026-03-cosmo3d.md) |
| 2026-01 | ReLi3D: 可重光照 3D 重建 | 3D Reconstruction | [主页](https://reli3d.jdihlmann.com/) · [笔记](papers/2026-01-reli3d.md) |
| 2025 | 3D Gaussian Map for VLN | VLA/VLN | [论文](https://openaccess.thecvf.com/content/ICCV2025/papers/Gao_3D_Gaussian_Map_with_Open-Set_Semantic_Grouping_for_Vision-Language_Navigation_ICCV_2025_paper.pdf) · [笔记](papers/2025-ICCV-3d-gaussian-map-vln.md) |
| 2025-11 | BuildingWorld: 全球 3D 建筑数据集 | 3D Reconstruction | [论文](https://arxiv.org/abs/2511.06337) · [笔记](papers/2025-11-buildingworld.md) |

---

## 📅 待读列表 (To Read)

- [ ] TerraScope: 像素级地理空间推理 VLM
- [ ] Fast-WAM: Do World Action Models Need Test-time Future Imagination?
- [ ] Towards Generalist Embodied AI: A Survey on World Models for VLA Agents
- [ ] awesome-world-models-for-vla-agents
- [ ] Uni-Walker: Lifelong Embodied Navigation Learning
- [ ] CoSMo3D: Open-World Promptable 3D Semantic Part Segmentation
- [ ] MeMix: 长时序 3D 重建方法
- [ ] BuildingWorld: 全球 3D 建筑数据集
- [ ] 3D Gaussian Map for VLN
- [ ] Hi-GRPO: RL 用于 3D 生成

---

## 📊 统计

| 领域 | 项目数 |
|------|--------|
| Vision / Geospatial | 1 |
| World Model | 1 |
| VLA/VLN | 3 |
| Embodied AI | 1 |
| 3D Generation | 2 |
| 3D Reconstruction | 3 |
| **总计** | **11** |

- **本月新增:** 11
- **已读:** 0 | **待读:** 11

---

## 📝 更新日志

| 日期 | 操作 | 内容 |
|------|------|------|
| 2026-03-27 | 新增论文 | TerraScope: 像素级地理空间推理 VLM (CVPR 2026) |
| 2026-03-25 | 新增论文 | Hi-GRPO: 首个系统性研究 RL 用于 3D 生成 (CVPR 2026) |
| 2026-03-25 | 新增论文 | 3D Gaussian Map for VLN (ICCV 2025) |
| 2026-03-25 | 优化排序 | 所有时间线改为从近到远排序 |
| 2026-03-25 | 新增论文 | BuildingWorld: 全球 3D 建筑数据集 |
| 2026-03-25 | 新增论文 | ReLi3D: 可重光照多视图 3D 重建 |
| 2026-03-24 | 重构分类 | 新增 VLA/VLN、3D Generation 领域，重新整理项目分类 |
| 2026-03-24 | 新增论文 | CoSMo3D: 开放世界 3D 语义部件分割 |
| 2026-03-24 | 新增论文 | Fast-WAM: 世界动作模型推理优化 |
| 2026-03-24 | 新增论文 | Uni-Walker: Lifelong Embodied Navigation Learning |
| 2026-03-24 | 初始创建 | 迁移桌面文档，建立 git 仓库 |