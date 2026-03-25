# 3D Gaussian Map with Open-Set Semantic Grouping for Vision-Language Navigation

## 基本信息

| 项目 | 内容 |
|------|------|
| **名称** | 3D Gaussian Map (3DGM) |
| **机构** | 待查证 |
| **时间** | ICCV 2025 |
| **链接** | [论文](https://openaccess.thecvf.com/content/ICCV2025/papers/Gao_3D_Gaussian_Map_with_Open-Set_Semantic_Grouping_for_Vision-Language_Navigation_ICCV_2025_paper.pdf) |
| **作者** | Gao 等 |

## 核心贡献

提出 **3D Gaussian Map (3DGM)**，结合 3D Gaussian Splatting 与开放集语义分组，用于视觉语言导航 (VLN) 任务，解决传统 VLN 方法在开放环境中的语义理解和导航泛化问题。

## 技术方法

### 3D Gaussian Map

- 基于 **3D Gaussian Splatting** 构建场景表示
- 支持高效的新视角合成和几何重建
- 为 VLN 提供丰富的空间和外观信息

### Open-Set Semantic Grouping

- **开放集语义理解**：支持未见过的语义类别
- **语义分组**：将 3D 高斯点按语义相似性分组
- 提升 VLN 指令中的语义对齐能力

### Vision-Language Navigation

- 将自然语言指令与 3D 场景关联
- 支持开放环境下的长程导航
- 提升对复杂指令的理解和执行能力

## 应用场景

- 室内机器人导航
- 具身智能体任务执行
- 开放环境 VLN
- 语义导航

## 实验结果

*待补充：需要阅读完整论文获取实验细节*

## 局限性

- ICCV 2025 新论文，代码和数据集可用性待确认
- 开放集语义分组的泛化能力需进一步验证

## 个人笔记

这是将 3D Gaussian Splatting 应用于 VLN 的早期工作之一，结合了神经渲染和具身导航两个热门方向。开放集语义分组是关键创新点，可能解决传统 VLN 方法在开放环境中的泛化瓶颈。

## 相关工作

- 3D Gaussian Splatting (SIGGRAPH 2023)
- Vision-Language Navigation (CVPR/ICCV 相关工作)
- Open-Vocabulary 语义分割

---

> 创建时间：2026-03-25
> 最后更新：2026-03-25
