# SparseNeuS

SparseNeuS: Fast Generalizable Neural Surface Reconstruction from Sparse Views

## 论文与官方资源

- [SparseNeuS: Fast Generalizable Neural Surface Reconstruction from Sparse Views](https://arxiv.org/abs/2206.05737) · [直接打开 PDF](https://arxiv.org/pdf/2206.05737)
- [会议全文 PDF](https://www.ecva.net/papers/eccv_2022/papers_ECCV/papers/136920210.pdf)

## 阅读标注

| 项目 | 内容 |
| --- | --- |
| 年份与发表信息 | ECCV 2022 |
| 优先级 | B 泛化模型进阶 |
| 训练方式 | 跨数据预训练与单对象微调结合 |
| 模板依赖 | 不依赖人体模板 |
| 项目关系 | 后续拓展 |

## 输入与输出

**输入：** 稀疏多视图照片和相机参数。

**输出：** 可泛化或微调后的 SDF 表面。

## 重点学习

1. 多视图特征到几何编码体积。
2. SDF 解码与粗到细推理。
3. 预训练泛化和单对象微调的成本与作用。

## 对 BodyTrace 的建议用途

探索少量照片快速生成自由人体表面的模型构造。

## 适用条件与边界

稀疏视图能力受视图重叠、相机、姿态与数据分布影响。

## 建议实践

分别评价不微调和固定预算微调，按人体身份隔离验证。

## 复现状态

论文和会议全文已核验；本资料包未核验完整训练复现。

[返回完整论文目录](../../README.md)

论文方法及原始资料按原学习索引保留；优先级和实践任务为项目学习建议。
