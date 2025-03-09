# ⚡ **TITAN Core**

![C++](https://img.shields.io/badge/lang-C%2B%2B17-blue)
![Realtime](https://img.shields.io/badge/realtime-1kHz-yellow)
![Platform](https://img.shields.io/badge/platform-linux--rt-informational)

> **Industrial motion controller for robotic arms.**

---

### Overview

TITAN Core provides deterministic control loops, path planning, and safety systems for multi-axis robotics.
Originally for research labs, now open for makers.

docs → [titan-core.dev](https://titan-core.dev)

---

### Build & Run

```bash
mkdir build && cd build
cmake ..
make
sudo ./titan_core --config demo.yaml
```

---

### Key Features

* 1kHz control loop
* 5-axis interpolation
* CANopen + Modbus drivers
* Safety interlocks

---

### Config snippet

```yaml
safety:
  e_stop_gpio: 27
  torque_limit: 1.2
planner:
  mode: spline
  tick_ms: 1
```

---

### Visualization

Works with [rosbridge](https://rosbridge.dev) and [rviz](https://rviz.dev)

---

### License & Credits

GPLv3 • Maintained by **R. Santos**

> "Built after debugging servo jitter for months."

# Touch update: 1760952549

# Touch update: 1760952550
