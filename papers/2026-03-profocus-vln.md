# ProFocus: Proactive Perception and Focused Reasoning in Vision-and-Language Navigation

**arXiv:** [2603.05530](https://arxiv.org/abs/2603.05530)  
**作者:** Wei Xue, Mingcheng Li, Xuecheng Wu, Jingqun Tang, Dingkang Yang, Lihua Zhang  
**发表:** CVPR 2026  
**领域:** Robotics (cs.RO), Computer Vision and Pattern Recognition (cs.CV)  
**提交日期:** 2026-02-28 (v1), 2026-03-14 (v2)  

---

## 核心问题

视觉语言导航(VLN)需要智能体准确感知复杂视觉环境并在导航指令和历史上下文中进行推理。现有方法存在两大痛点：

1. **被动感知冗余**: 被动处理全景视觉输入，包含大量无关信息，导致感知效率低下
2. **历史上下文无差别处理**: 对所有历史航点一视同仁，导致注意力分散、推理不聚焦

## 方法概述

提出 **ProFocus**——一个**无需训练**的渐进式框架，首次将主动感知和聚焦推理统一应用于VLN任务，通过LLM与VLM协作实现：

### 1. 推理引导的主动感知 (Proactive Perception)

- 将全景观测转化为**结构化自我中心语义地图**(ego-centric semantic maps)
- 编排代理(orchesration agent)识别决策所需的缺失视觉信息
- 生成带焦点区域的定向视觉查询，引导感知代理获取所需观测
- 构建**感知-推理闭合循环**，迭代获取与导航指令相关的视觉观测

### 2. 分支多样化蒙特卡洛树搜索 (BD-MCTS)

- 从海量历史候选航点中筛选 **top-k 高价值航点**
- 决策模型仅聚焦于这些航点的关联上下文进行推理
- 解决历史上下文无差别处理导致的注意力分散问题

## 关键特性

| 特性 | 说明 |
|------|------|
| 无需训练 | Training-free，无需任务特定调优 |
| 部署便捷 | 直接利用预训练LLM/VLM能力 |
| 渐进式框架 | 感知-推理闭环迭代优化 |
| 零样本SOTA | R2R 和 REVERIE 基准上零样本方法最佳 |

## 实验结果

在 **R2R** 和 **REVERIE** 基准测试中，达到所有**零样本方法中的 SOTA** 性能。

## 意义

- 首次统一主动感知与聚焦推理于VLN任务
- 摒弃传统被动处理全景输入的范式
- 为无需微调的VLN系统提供了新方向

---

## 相关链接

- **论文:** https://arxiv.org/abs/2603.05530
- **PDF:** https://arxiv.org/pdf/2603.05530
- **HTML:** https://arxiv.org/html/2603.05530v2
