# Verilog / SystemVerilog

> 状态：🚧 整理中

## 推荐教材

- **《Verilog HDL》** — Samir Palnitkar（入门经典）
- **《SystemVerilog for Verification》** — Chris Spear（验证必读）
- **《数字集成电路：电路、系统与设计》** — Rabaey

## 推荐网课 / 资源

- HDLBits — <https://hdlbits.01xz.net/>（在线练习神器，必刷）
- Coursera：Hardware Description Languages for FPGA Design

## 学习要点

- [ ] 模块、端口、wire / reg
- [ ] 阻塞 / 非阻塞赋值的区别
- [ ] always 块的三种典型用法
- [ ] 有限状态机（FSM）写法
- [ ] 可综合 vs 不可综合代码
- [ ] SystemVerilog：interface、class、覆盖率、断言

## 一个最简示例

```verilog
module counter #(parameter WIDTH = 4) (
    input  logic              clk,
    input  logic              rst_n,
    output logic [WIDTH-1:0]  cnt
);
    always_ff @(posedge clk or negedge rst_n) begin
        if (!rst_n) cnt <= '0;
        else        cnt <= cnt + 1'b1;
    end
endmodule
```
