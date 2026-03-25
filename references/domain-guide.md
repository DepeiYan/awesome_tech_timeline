# 技术领域分类指南

## 领域定义与关键词

### World Model (世界模型)
- **定义**: 学习环境的内部表示，用于预测、规划和决策
- **关键词**: World Model, World Action Model, WAM, Model-based RL, Dynamics Model
- **典型任务**: 未来状态预测、动作规划、策略学习

### VLA/VLN (视觉语言动作/导航)
- **定义**: 结合视觉、语言和动作的具身智能系统
- **关键词**: Vision-Language-Action, VLN, Embodied Navigation, Robot Instruction
- **典型任务**: 视觉导航、语言指令执行、机器人操作

### Embodied AI (具身智能)
- **定义**: 智能体在物理环境中感知、行动和学习
- **关键词**: Embodied, Robot Learning, Navigation, Manipulation, Simulation
- **典型任务**: 导航、抓取、交互、探索

### 3D Reconstruction (3D重建)
- **定义**: 从图像、点云等数据重建3D几何和外观
- **关键词**: SLAM, NeRF, 3D Reconstruction, Gaussian Splatting, Multi-view, Structure from Motion
- **典型任务**: 场景重建、物体重建、位姿估计

### 3D Generation (3D生成)
- **定义**: 从文本、图像等生成3D内容
- **关键词**: 3D Generation, Text-to-3D, Image-to-3D, 3D Editing, Neural Rendering
- **典型任务**: 3D建模、纹理生成、形状编辑

### Diffusion (扩散模型)
- **定义**: 基于扩散过程的生成模型
- **关键词**: Diffusion, DDPM, Stable Diffusion, Image Generation, Video Generation
- **典型任务**: 图像生成、视频生成、图像编辑

### LLM (大语言模型)
- **定义**: 大规模预训练语言模型
- **关键词**: LLM, GPT, Language Model, Transformer, Prompt, Fine-tuning
- **典型任务**: 文本生成、问答、推理、代码生成

### Vision (计算机视觉)
- **定义**: 图像和视频的理解与分析
- **关键词**: Object Detection, Segmentation, Classification, Tracking, CV
- **典型任务**: 目标检测、语义分割、图像分类

### RL (强化学习)
- **定义**: 通过与环境交互学习最优策略
- **关键词**: Reinforcement Learning, RL, Policy, Q-learning, Actor-Critic, PPO
- **典型任务**: 游戏、机器人控制、决策优化

## 判断规则

1. **优先匹配最具体的领域**：如同时涉及 VLA 和 World Model，优先 VLA
2. **多标签处理**：跨领域工作可在多个领域文件中记录，但主笔记放在最相关领域
3. **新兴领域**：遇到新领域时，在 INDEX.md 中新增分类

## 领域交叉示例

| 论文主题 | 主领域 | 次领域 |
|----------|--------|--------|
| VLA + World Model | VLA/VLN | World Model |
| 3D Generation + Diffusion | 3D Generation | Diffusion |
| Embodied Navigation + RL | Embodied AI | RL |
| NeRF + SLAM | 3D Reconstruction | Vision |

---

> 最后更新: 2026-03-25