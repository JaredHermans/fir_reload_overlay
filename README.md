## Coefficient Re-loadable FIR Filter in Zynq-7000
This repository demonstrates the hardware and software design for a coefficient re-loadable FIR filter in the PL. The project is demonstrated on a Pynq-Z2 board running PYNQ. Performance is compared to a software only FIR filter.

**./fir_reload** - Vivado project for re-loadable FIR filter.

**./notebook** - Jupyter notebook running on the Pynq-Z2

**./overlay** - PYNQ fir_reload overlay. Copy files to /home/xilinx/overlays/fir_reload on the Pynq-Z2 board. Also contains FIR filter coefficients.

**fir.mlx** - MATLAB live script used to generate the FIR filter coefficients.

**high_pass_coef.coe** + **low_pass_coef.coe** - Coefficent files for FIR Compiler IP in Vivado.

**bit.sh** - Bash script to copy bitstream and hardware description from Vivado project to overlay directory

References: [FPGAdeveloper](https://www.fpgadeveloper.com/2018/03/how-to-accelerate-a-python-function-with-pynq.html/) and [RFSoC_DSP](https://github.com/Xilinx/DSP-PYNQ)
