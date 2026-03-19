## Transformer核心结构

Transformer的核心公式：$Attention(Q, K, V) = softmax(\frac{QK^T}{\sqrt{d_k}})V$

其中Q代表查询，K代表键，V代表值，所谓注意力就是$QKV$。

## Transformer为什么比RNN/CNN更适合长距离依赖

## self-attention在做什么

## Attention和self-attention之间的区别

Attention是一种让模型对不同信息分配不同权重的机制，本质上是按信息相关性聚合信息。它的$Q,K,V$可以来自不同地方。

self-attention属于Attention，是Attention的一种特殊形式，它的$Q,K,V$都来自相同的序列，让模型更加关注自身 ，这使得Transformer相比于传统的RNN来说更适合处理长距离依赖问题。

## multi-head attention的作用

## encode/decode 结构

