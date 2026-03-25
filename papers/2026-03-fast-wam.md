# Fast-WAM: Do World Action Models Need Test-time Future Imagination?

## 📋 基本信息

| 字段 | 内容 |
|------|------|
| **标题** | Fast-WAM: Do World Action Models Need Test-time Future Imagination? |
| **作者** | Tianyuan Yuan, Zibin Dong, Yicheng Liu, Hang Zhao |
| **来源** | arXiv |
| **发表时间** | 2026-03-17 (v1), 2026-03-23 (v2) |
| **arXiv ID** | 2603.16666 |
| **类型** | 研究论文 |
| **领域** | World Action Models / 具身智能 |

## 🔗 链接

- 📖 [论文链接](https://arxiv.org/abs/2603.16666)
- 🌐 [项目主页](https://yuantianyuan01.github.io/FastWAM/)
- 🐙 代码仓库：_待补充_

---

## 🌟 核心贡献

**质疑 WAM 的 test-time future imagination 必要性**，提出 Fast-WAM 架构，保留训练时的视频建模但跳过推理时的未来预测，实现 4 倍加速且性能相当。

### 主要创新

1. **问题定义**
   - 现有 WAM 采用 imagine-then-execute 范式，推理时视频去噪带来高延迟
   - 质疑：显式未来想象是否真的必要？

2. **Fast-WAM 架构**
   - 训练时保留视频 co-training
   - 推理时跳过未来预测
   - 实现 190ms 延迟，比现有 WAM 快 4 倍以上

3. **关键发现**
   - Fast-WAM 与 imagine-then-execute 变体性能相当
   - 移除视频 co-training 导致性能大幅下降
   - 视频预测的主要价值在于训练时改善世界表征，而非推理时生成未来观测

---

## 📊 性能指标

- **推理延迟**: 190ms (实时)
- **速度提升**: 4 倍以上（相比现有 imagine-then-execute WAMs）
- **测试基准**: LIBERO, RoboTwin
- **无需具身预训练**即可达到 SOTA 效果

---

## 💭 笔记/心得

> _待阅读后补充_

---

## 🏷️ 标签

#WorldActionModel #WAM #VLA #具身智能 #实时推理 #视频预测

---

**收录时间:** 2026-03-24  
**状态:** 📅 待读
