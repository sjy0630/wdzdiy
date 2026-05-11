# Python

> 状态：🚧 整理中

## 推荐教材

- **《Python Crash Course》** — Eric Matthes
- **《流畅的 Python》** — Luciano Ramalho（进阶必读）

## 推荐网课

- 中国大学 MOOC：嵩天《Python 语言程序设计基础》
- Real Python — <https://realpython.com/>

## 学习要点

- [ ] 基础语法、列表 / 字典 / 字符串
- [ ] 函数、模块、面向对象
- [ ] 文件 IO、异常处理
- [ ] NumPy / SciPy / Matplotlib
- [ ] Pandas（数据处理）
- [ ] 正则表达式、subprocess（脚本化关键）

## 在微电子中的典型用途

```python
# 仿真结果后处理：读取 spice .csv 输出，画 PSD
import pandas as pd
import numpy as np
import matplotlib.pyplot as plt

df = pd.read_csv("sim.csv")
f, psd = welch(df["v_out"].values, fs=1e9)
plt.semilogy(f, psd)
plt.xlabel("Frequency (Hz)")
plt.ylabel("PSD (V²/Hz)")
plt.show()
```

- **EDA 脚本化** — 自动批量跑仿真、Corner、Monte Carlo
- **报告生成** — 用 Jupyter Notebook 整理实验数据
- **机器学习辅助设计** — 工艺角分类、电路自动尺寸
