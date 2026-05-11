# FPGA 与 Vivado

> 状态：🚧 整理中

## 推荐教材

- **《FPGA Prototyping by SystemVerilog Examples》** — Pong Chu
- **《Digital Design and Computer Architecture》** — Harris（含 FPGA 实验）

## 推荐板卡

| 价位 | 板卡 | 适用 |
| --- | --- | --- |
| 入门 | 黑金 / 米联客 Artix-7 | 学 Verilog、跑流水灯 / UART |
| 进阶 | Xilinx Zynq-7020 | ARM + FPGA，跑 Linux + 加速器 |
| 高端 | Kintex / UltraScale | 高速 SerDes、AI 加速 |

## 学习要点

- [ ] Vivado 工程创建与综合 / 实现
- [ ] 时钟约束（XDC）
- [ ] IP Catalog（PLL / FIFO / Block RAM）
- [ ] ChipScope / ILA 在线调试
- [ ] 简单项目：UART → SPI → VGA → 简易 RISC-V

## 进阶方向

- **HLS**（High Level Synthesis）：用 C/C++ 写硬件
- **ZYNQ SoC**：嵌入式 Linux + PL 加速
- **AXI 总线**：理解片上互连标准
