# Tuya Data Points

## [LinkTree](https://linktr.ee/DzurisHome)

[![ko-fi](https://ko-fi.com/img/githubbutton_sm.svg)](https://ko-fi.com/DzurisHome)

</br>

> [!CAUTION]
> Version 3.1 (and some 3.3) - Plug or Switch Type

| DP ID | Function Point | Type     | Range     | Units     |
|------ | --------------- | -------- | --------- | --------- |
| 1     | Switch          | bool     | True/False|           |
| 2     | Countdown?      | integer  | 0-86400   | s         |
| 4     | Current         | integer  | 0-30000   | mA        |
| 5     | Power           | integer  | 0-50000   | W         |
| 6     | Voltage         | integer  | 0-5000    | V         |

</br>

> [!CAUTION]
> Version 3.1 - Light Type (RGB)

| DP ID | Function Point | Type      | Range                    | Units    |
|------ | --------------- | --------- | ------------------------ | -------- |
| 1     | Switch          | bool      | True/False               |          |
| 2     | Mode            | enum      | white, colour, scene, music|         |
| 3     | Bright          | integer   | 10-1000*                 |          |
| 4     | Color Temp      | integer   | 0-1000*                  |          |
| 5     | Color           | hexstring | r:0-255, g:0-255, b:0-255, h:0-360, s:0-255, v:0-255 | rgb+hsv |

</br>

> [!CAUTION]
> Version 3.3 Devices
> 
> Version 3.3 - Plug, Switch, Power Strip Type |

| DP ID | Function Point | Type     | Range     | Units     |
|------ | --------------- | -------- | --------- | --------- |
| 1     | Switch 1        | bool     | True/False|           |
| 2     | Switch 2        | bool     | True/False|           |
| 3     | Switch 3        | bool     | True/False|           |
| 4     | Switch 4        | bool     | True/False|           |
| 5     | Switch 5        | bool     | True/False|           |
| 6     | Switch 6        | bool     | True/False|           |
| 7     | Switch 7/usb    | bool     | True/False|           |
| 9     | Countdown 1     | integer  | 0-86400   | s         |
| 10    | Countdown 2     | integer  | 0-86400   | s         |
| 11    | Countdown 3     | integer  | 0-86400   | s         |
| 12    | Countdown 4     | integer  | 0-86400   | s         |
| 13    | Countdown 5     | integer  | 0-86400   | s         |
| 14    | Countdown 6     | integer  | 0-86400   | s         |
| 15    | Countdown 7     | integer  | 0-86400   | s         |
| 17    | Add Electricity | integer  | 0-50000   | kWh       |
| 18    | Current         | integer  | 0-30000   | mA        |
| 19    | Power           | integer  | 0-50000   | W         |
| 20    | Voltage         | integer  | 0-5000    | V         |
| 21    | Test Bit        | integer  | 0-5       | n/a       |
| 22    | Voltage coeff.  | integer  | 0-1000000 |           |
| 23    | Current coeff.  | integer  | 0-1000000 |           |
| 24    | Power coeff.    | integer  | 0-1000000 |           |
| 25    | Electricity coeff. | integer | 0-1000000 |         |
| 26    | Fault           | fault    | ov_cr     |           |
| 38    | Power-on state setting | enum | off, on, memory |    |
| 39    | Overcharge Switch | bool | True/False |           |
| 40    | Indicator status setting | enum | none, on, relay, pos | |
| 41    | Child Lock      | bool     | True/False|           |
| 42    | UNKNOWN         |          |           |           |
| 43    | UNKNOWN         |          |           |           |
| 44    | UNKNOWN         |          |           |           |

> [!NOTE]
> Note: Some 3.3 energy management plugs use the DPS values of the 3.1 plug above.

</br>

> [!CAUTION]
> Version 3.3 - Dimmer Switch

| DP ID | Function Point | Type     | Range     | Units     |
|------ | --------------- | -------- | --------- | --------- |
| 1     | Switch          | bool     | True/False|           |
| 2     | Brightness      | integer  | 10-1000* |           |
| 3     | Minimum of Brightness | integer | 10-1000* |       |
| 4     | Type of light source1 | enum | LED, incandescent, halogen | |
| 5     | Mode            | enum     | white     |           |

</br>

> [!CAUTION]
> Version 3.3 - Light Type (RGB)

| DP ID | Function Point | Type     | Range     | Units     |
|------ | --------------- | -------- | --------- | --------- |
| 20    | Switch          | bool     | True/False|           |
| 21    | Mode            | enum     | white, colour, scene, music | |
| 22    | Bright          | integer  | 10-1000* |           |
| 23    | Color Temp      | integer  | 0-1000   |           |
| 24    | Color           | hexstring | h:0-360, s:0-1000, v:0-1000 | hsv |
| 25    | Scene           | string   | n/a       |           |
| 26    | Left time       | integer  | 0-86400  | s         |
| 27    | Music           | string   | n/a       |           |
| 28    | Debugger        | string   | n/a       |           |
| 29    | Debug           | string   | n/a       |           |

</br>

> [!CAUTION]
> Version 3.3 - Automated Curtain Type

| DP ID | Function Point         | Type    | Range          | Units |
|------ | ---------------------- | ------- | --------------- | ----- |
| 1     | Curtain Switch 1      | enum    | open, stop, close, continue | |
| 2     | Percent control 1     | integer | 0-100           | %     |
| 3     | Accurate Calibration 1 | enum    | start, end      |       |
| 4     | Curtain Switch 2      | enum    | open, stop, close, continue | |
| 5     | Percent control 2     | integer | 0-100           | %     |
| 6     | Accurate Calibration 2 | enum    | start, end      |       |
| 8     | Motor Steer 1         | enum    | forward, back   |       |
| 9     | Motor steer 2         | enum    | forward, back   |       |
| 10    | Quick Calibration 1    | integer | 1-180           | s     |
| 11    | Quick Calibration 2    | integer | 1-180           | s     |
| 12    | Motor Mode 1          | enum    | strong_power, dry_contact | |
| 13    | Motor Mode 2          | enum    | strong_power, dry_contact | |
| 14    | Light mode            | enum    | relay, pos, none |       |

</br>

> [!CAUTION]
> Version 3.3 - Fan Switch Type

| DP ID | Function Point        | Type    | Range        | Units |
|------ | --------------------- | ------- | -----------   | ----- |
| 1     | Fan switch            | bool    | True/False   | n/a   |
| 2     | Fan countdown         | integer | 0-86400      | s     |
| 3     | Fan speed             | enum    | level_1, level_2, level_3, level_4, level_5 | |
| 4     | Fan speed             | integer | 1-100        | %     |
| 5     | Fan light switch      | bool    | True/False   |       |
| 6     | Brightness            | integer | 10-1000      |       |
| 7     | Fan light countdown    | integer | 0-86400      | s     |
| 8     | Minimum brightness    | integer | 10-1000      |       |
| 9     | Maximum brightness    | integer | 10-1000      |       |
| 10    | Mode                  | enum    | white        |       |
| 11    | Power-on state setting | enum    | off, on, memory |     |
| 12    | Indicator status setting | enum  | none, relay, pos |       |
| 13    | Backlight switch      | bool    | True/False   |       |

</br>

> [!CAUTION]
> Version 3.3 - Universal IR Controller with optional Temp/Humidity

| DP ID | Function Point         | Type    | Range        | Units |
|------ | ---------------------- | ------- | -----------   | ----- |
| 101   | Current Temperature    | integer | 0-600        | 10x Celsius |
| 102   | Current Humidity       | integer | 0-100        | %     |
| 201   | IR Commands (set only) | JSON*   | n/a          | n/a   |

## [LinkTree](https://linktr.ee/DzurisHome)

[![ko-fi](https://ko-fi.com/img/githubbutton_sm.svg)](https://ko-fi.com/DzurisHome)
