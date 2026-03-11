---
tags:
  - Transformer
  - NLP
  - Attention
---

# Attention Is All You Need

| 信息 | 内容 |
|------|------|
| **作者** | Vaswani et al. |
| **发表** | NeurIPS 2017 |
| **链接** | [arXiv:1706.03762](https://arxiv.org/abs/1706.03762) |

## 一句话总结

提出 Transformer 架构，完全基于 self-attention 机制，摒弃了 RNN 和 CNN。

## 核心思想

Scaled Dot-Product Attention：

\[
\text{Attention}(Q, K, V) = \text{softmax}\left(\frac{QK^T}{\sqrt{d_k}}\right)V
\]

其中 \(d_k\) 是 key 的维度，除以 \(\sqrt{d_k}\) 防止点积过大导致 softmax 饱和。

## 关键贡献

1. **Self-Attention 替代循环** — 并行计算，训练更快
2. **Multi-Head Attention** — 不同子空间捕获不同模式
3. **Positional Encoding** — 用正弦函数注入位置信息

## 我的思考

!!! note "个人理解"
    这里写你自己对论文的思考、疑问、与其他工作的联系等。

## 相关论文

- BERT (Devlin et al., 2018)
- GPT (Radford et al., 2018)
