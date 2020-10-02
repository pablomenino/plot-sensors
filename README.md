<h3 align="center">plot-sensors</h3>
<p align="center">Graph Thermal Sensor Data with BASH and GNUPlot</p>

<p align="center">
<img src="https://img.shields.io/github/release/pablomenino/plot-sensors.svg">
<img src="https://img.shields.io/github/license/pablomenino/plot-sensors.svg">
</p>

**Graph Thermal Sensor Data with BASH and GNUPlot**

![ScreenShot](https://raw.githubusercontent.com/pablomenino/plot-sensors/master/examples/cpu.png)

![ScreenShot](https://raw.githubusercontent.com/pablomenino/plot-sensors/master/examples/gpu.png)


## Table of contents

* [How to Use](#how-to-use)
* [Known Bugs](#known-bugs)
* [Credit](#credit)

## <a name="how-to-use">How to Use

#### Requirements

* BASH
* GNU Plot
* nVidia drivers for GPU

#### Usage

Log temperature over some time  interval given as days, hours, minutes or seconds.

Enter the variables according to usage:

duration="$1"  #duration format is  ndnhnmns where n is some number and d is day,

h is hours, m is minutes and s is seconds. For example, 4d , 4d5h30m , 5m30s, 6h30m30s are all valid.

**Example for CPU:**

```bash
# ./plot-cpu.sh 2h 5s
```
Run for 2 hours, and get CPU temp values every 5 seconds.

**Example for GPU:**

```bash
# ./plot-gpu.sh 30m 1s
```

Run for 30 minutes, and get GPU temp value every 1 second.

## <a name="credit">Credit

* **Script based on:** [where-can-i-find-the-log-file-of-my-system-temperature](https://askubuntu.com/questions/96957/where-can-i-find-the-log-file-of-my-system-temperature)
