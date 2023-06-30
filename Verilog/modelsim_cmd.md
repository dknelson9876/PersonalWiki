# Modelsim Commands from Tutorial

## Commands run by the GUI

- Generating the project:
    - `vlib work`
    - `vmap work work`
- Compile verilog files:
    - `vlog -reportprogress 300 -work work [file]
- Load the simulation:
    - `vsim work.test_counter`
- Add test signals to the wave window:
    - `add wave -position insertpoint sim:/test_counter/*`
- Start the sim:
    - `run` (for the default time)
    - `run 500` (for 500 ns)
    - `run -all` (until stopped)