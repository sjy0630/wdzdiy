# Tcl / Make 脚本

> 状态：🚧 整理中

## 为什么要学

EDA 工具链（DC / ICC2 / PrimeTime / Innovus）几乎全部基于 **Tcl** 控制；
项目自动化（批量仿真、回归测试）通常用 **Makefile** 串起来。

## Tcl

### 推荐资源

- **《Tcl/Tk 入门经典》** — Brent Welch
- **Synopsys Tcl Reference**（DC/ICC2 工具自带）

### 学习要点

- [ ] 变量、列表、字典
- [ ] 控制流、过程
- [ ] 文件 IO
- [ ] DC / PT 中常用命令套路（read_verilog / link / compile / report_timing）

## Make

### 推荐资源

- **GNU Make Manual** — <https://www.gnu.org/software/make/manual/>
- **Managing Projects with GNU Make** — Robert Mecklenburg

### 学习要点

- [ ] 目标 / 依赖 / 命令
- [ ] 隐式规则与模式规则
- [ ] 变量、函数、`$@`/`$<`/`$^`
- [ ] 多目标并行（`make -j`）

## 典型 Makefile 范式

```makefile
TOP      = top
RTL      = $(wildcard rtl/*.v)
TB       = $(wildcard tb/*.v)
SIMULATOR = vcs

sim:
	$(SIMULATOR) -full64 -sverilog $(RTL) $(TB) -o simv
	./simv

clean:
	rm -rf simv* csrc DVEfiles
```
