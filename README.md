
# plc-examples

Some very basic examples I run on S7-314C-2 DP. I only use this repo as a personal backup, but I made it public.

- [pass](pass-OB1.stl): press 3 buttons in correct order (0-2-1) and green led turns on.
- [sliding light](sliding-light-OB35.stl): sliding output (light if powered) on one output bank
- [double sliding light with onoff](double-sliding-light-with-onoff-ob35.stl): sliding output on two digial output banks controlled with two digital inputs

# S7-314C-2 DP

## Integrated I/O default addresses

The right integrated module:
- 16x digital inputs: 124.0-125.7
- 16x digital outputs: 124.0-125.7

The left integrated module:
- 8x digital inputs: 126.0-126.7
- 4x analog in:
- 1x analog R in:
- 2x analog out:

## Wiring Notes

Digital outputs common L (24V) and M (GND) should be connected. Digital load is connected between the digital output and GND. Digital outputs do output 24V.
Digital inputs common L (24V) and M (GND) should be connected. ON is 24V at digital inputs e.g. a switch/pushbutton connected between 24V and a digital input.
