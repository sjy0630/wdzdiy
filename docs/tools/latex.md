# LaTeX

> 状态：🚧 整理中

## 为什么要学

- 实验报告 / 课程论文 / 毕业论文
- 投稿 IEEE / ACM 期刊
- 复杂公式（电路传递函数、噪声推导）排版

## 推荐资源

- **Overleaf** — <https://www.overleaf.com/>（在线即可使用）
- **《LaTeX 入门》** — 刘海洋
- LearnLaTeX — <https://www.learnlatex.org/zh-cn/>

## 学习要点

- [ ] 文档结构：article / report / book
- [ ] 数学公式（amsmath）
- [ ] 图片、表格、参考文献（BibTeX）
- [ ] IEEE / ACM 模板使用
- [ ] TikZ 画电路图（circuitikz）

## 微电子场景示例

```latex
\usepackage{circuitikz}
\begin{circuitikz}
  \draw (0,0) to[V, l=$V_{in}$] (0,2)
        to[R, l=$R$] (2,2)
        to[C, l=$C$] (2,0) -- (0,0);
\end{circuitikz}
```
