# G-Code Force Mapper

A browser-based utility for mapping dynamometer CSV data onto ISO G-code 
toolpaths to identify the specific block with high peak force, moment or user defined data.

## What it does

Upload an ISO G-code file and a dynamometer or any other user defined data. The tool aligns your 
cutting forces (Fx, Fy, Fz), torque (Mz), and any user-defined data 
channel to the toolpath geometry. It returns the exact G-code line number, 
XYZ location, and confidence for the peak force event.

No installation. Runs in the browser.

## Typical use

- Find the toolpath block that caused high forces, moment etc.
- Cutting condition comparison — same G-code, different CSV files, compare 
  peak force locations across runs
- Custom data mapping — map vibration, temperature, acoustics, or 
  any time-series signal onto the toolpath alongside force channels

## Compatibility

- ISO dialects
- 3-axis machining
- Not supported: 3+2 and simultaneous 5-axis, Heidenhain Klartext, Mazatrol, 
  subprogram expansion, canned cycles, G95 feed per revolution

## Launch

[Open Web Utility](https://gcode-map.streamlit.app)

[Full documentation and scope](https://gcodemap.github.io/gcode-data-mapper/)

## Disclaimer

Free research utility. Output is for guidance only and does not replace 
professional engineering judgment or verified CAM simulation. No liability 
accepted for machine damage, tool breakage, part scrap, or financial loss.
