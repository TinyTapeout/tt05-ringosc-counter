all: sim

sim: osc.spice
	# run the simulation
	echo ".lib '$(PDK_ROOT)/sky130A/libs.tech/ngspice/sky130.lib.spice' tt" > pdk_lib.spice
	echo ".include '$(PDK_ROOT)/sky130A/libs.ref/sky130_fd_sc_hd/spice/sky130_fd_sc_hd.spice'" >> pdk_lib.spice
	ngspice $^
