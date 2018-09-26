# Unified control/status register
10 register values.

control: 9 downto 1 is used for PS to PL; register 0 is for interrupt handling

status: 7 downto 1 is used for PL to PS; 9 downto 8 is for device DNA; 0 for interrupt handling

tested using Koheron SDK. Interrupt yet to be tested and is not fully implemented yet.

Note: you cannot read the control signals from PS. they are handled by a seperate set of registers which are not wired to be read by the PS

AKG: DNA reader source code taken from koheron SDK
