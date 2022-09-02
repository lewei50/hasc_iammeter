# IamMeter

------

[IAMMETER](https://www.iammeter.com/) provides both a bi-directional single-phase energy meter([WEM3080](https://www.iammeter.com/products/single-phase-meter)) and a bi-directional three-phase energy monitor ([WEM3080T](https://www.iammeter.com/products/three-phase-meter)). Both of them can be integrated into Home Assistant.

## Configuration

Install iammeter integration by searching "iammeter" in HACS first.
Install iammeter device using Config Flow UI.

### CONFIGURATION VARIABLES

**host** string REQUIRED

The IP address of your IAMMETER.

**port** integer (optional, default: 80)

port of your IAMMETER.

**name** string (optional, default: IamMeter)

Name for the sensor entity.

## Sensors

Sensors available in the library:

### SINGLE-PHASE ENERGY METER (WEM3080/WEM3162)

| name                 | Unit | Description                  |
| :------------------- | :--- | :--------------------------- |
| wem3080_voltage      | V    | Voltage.                     |
| wem3080_current      | A    | current.                     |
| wem3080_power        | W    | active power.                |
| wem3080_importenergy | kWh  | Energy consumption from grid |
| wem3080_exportgrid   | kWh  | Energy export to grid        |

### THREE-PHASE ENERGY METER (WEM3080T)

| name                    | Unit | Description           |
| :---------------------- | :--- | :-------------------- |
| wem3080t_voltage_a      | V    | A phase voltage       |
| wem3080t_current_a      | A    | A phase current       |
| wem3080t_power_a        | W    | A phase active power  |
| wem3080t_importenergy_a | kWh  | A phase import energy |
| wem3080t_exportgrid_a   | kWh  | A phase export energy |
| wem3080t_frequency_a    | Hz   | A phase frequency     |
| wem3080t_pf_a           |      | A phase power factor  |
|                         |      |                       |
| wem3080t_voltage_b      | V    | B phase voltage       |
| wem3080t_current_b      | A    | B phase current       |
| wem3080t_power_b        | W    | B phase active power  |
| wem3080t_importenergy_b | kWh  | B phase import energy |
| wem3080t_exportgrid_b   | kWh  | B phase export energy |
| wem3080t_frequency_b    | Hz   | B phase frequency     |
| wem3080t_pf_b           |      | B phase power factor  |
|                         |      |                       |
| wem3080t_voltage_c      | V    | C phase voltage       |
| wem3080t_current_c      | A    | C phase current       |
| wem3080t_power_c        | W    | C phase active power  |
| wem3080t_importenergy_c | kWh  | C phase import energy |
| wem3080t_exportgrid_c   | kWh  | C phase export energy |
| wem3080t_frequency_c    | Hz   | C phase frequency     |
| wem3080t_pf_c           |      | C phase power factor  |
