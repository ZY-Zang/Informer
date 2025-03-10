# Informer for Multivariate Time Series Forecasting

[![PyTorch](https://img.shields.io/badge/PyTorch-1.8+-red.svg)](https://pytorch.org/)
[![License](https://img.shields.io/badge/License-MIT-blue.svg)](LICENSE)

本项目完整实现了Informer模型在ETTh1数据集上的多元时间序列预测，包含数据预处理、模型训练、预测评估的全流程代码。

## 主要特性

- ​**标准数据预处理**  
  ✅ 支持标准化/反标准化  
  ✅ 自动划分训练/验证/测试集（14/4/4月）  
  ✅ 时间特征编码（小时/周/月/假日）

- ​**模型架构**  
  🧠 ProbSparse自注意力机制  
  🧠 编码器-解码器架构（含注意力蒸馏）  
  🧠 自适应混合精度训练

- ​**高效实现**  
  ⚡ PyTorch原生实现  
  ⚡ 多GPU并行支持  
  ⚡ 预训练模型快速推理

## 环境依赖

- Python 3.7+
- PyTorch 1.8+
- pandas >=1.2
- numpy >=1.19
- scikit-learn

```bash
pip install -r requirements.txt