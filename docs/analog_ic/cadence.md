# Cadence Virtuoso 入门

> 状态：🚧 整理中

## 工具简介

Cadence Virtuoso 是模拟 / 混合信号 IC 设计的**业界标准平台**，包含：

- **Schematic Editor** — 画原理图
- **ADE (Analog Design Environment)** — 仿真环境
- **Spectre** — SPICE 类仿真器
- **Layout XL** — 版图设计
- **Calibre / Assura** — DRC / LVS 物理验证

## 学习资源

- **Cadence University Program** 官方教程
- B 站 / YouTube：搜 "Cadence Virtuoso tutorial"
- **Razavi 配套实验** — 每章后的电路都可以在 Cadence 里复现

## 上手要点

- [ ] Library Manager 与工艺库的概念
- [ ] 原理图绘制、Symbol 创建
- [ ] DC / AC / Tran / Noise / Monte Carlo 仿真
- [ ] 参数扫描（Parametric Sweep）与 Corner 仿真
- [ ] Layout 入门：器件匹配、对称性、Guard Ring
- [ ] DRC / LVS 流程

## 工艺 PDK

学校或实验室通常有 SMIC / TSMC / GF 等 PDK。如果个人学习，可以使用：

- **SkyWater 130nm 开源 PDK** — <https://skywater-pdk.readthedocs.io/>
- **GF 180nm 开源 PDK**
- **Magic + Xschem + Ngspice + Netgen** — 全开源 EDA 替代方案
