# 🚀 Week 0: RISC‑V Reference SoC Tapeout Program – Foundation & Tool Setup

Welcome to my **RISC‑V Reference SoC Tapeout Program** repository!
Week 0 was all about **setting up the environment and essential open-source tools** for the upcoming RTL-to-GDS design journey.
The focus was on ensuring a **stable workspace** to handle synthesis, simulation, circuit analysis, and layout tasks.

---

## 🎯 System & Virtual Machine Setup

| Specification 💻        | Details 📋    |
| ----------------------- | ------------- |
| **Operating System 🐧** | Ubuntu 20.04+ |
| **RAM 💾**              | 6 GB          |
| **Storage 💿**          | 50 GB HDD     |
| **vCPUs ⚡**             | 4             |

💡 *This configuration ensures smooth performance for toolchains, synthesis, and simulation.*

---

## ⚙️ Tools Installed

The following open-source VLSI tools were installed & verified:

| Tool                             | Status     | Purpose             |
| -------------------------------- | ---------- | ------------------- |
| 🧠 **Yosys**                     | ✅ Complete | RTL Synthesis       |
| 📟 **Icarus Verilog (Iverilog)** | ✅ Complete | Verilog Simulation  |
| 📊 **GTKWave**                   | ✅ Complete | Waveform Debugging  |
| ⚡ **Ngspice**                    | ✅ Complete | Circuit Simulation  |
| 🎨 **Magic VLSI**                | ✅ Complete | Layout Design & DRC |

---

### 🧠 Yosys – RTL Synthesis Tool

**Installation**

```bash
git clone https://github.com/YosysHQ/yosys.git
cd yosys
sudo apt install make build-essential clang bison flex \
libreadline-dev gawk tcl-dev libffi-dev git graphviz \
xdot pkg-config python3 libboost-system-dev \
libboost-python-dev libboost-filesystem-dev zlib1g-dev
make
sudo make install
```

✅ Verified with `yosys` command

---

### 📟 Iverilog – Verilog Simulator

**Installation**

```bash
sudo apt-get install iverilog
```

✅ Verified with `iverilog -v`

---

### 📊 GTKWave – Waveform Viewer

**Installation**

```bash
sudo apt-get install gtkwave
```

✅ Verified with `gtkwave`

---

### ⚡ Ngspice – Circuit Simulator

**Installation**

```bash
sudo apt-get install ngspice
```

✅ Verified with `ngspice -v`

---

### 🎨 Magic VLSI – Layout Tool

**Installation**

```bash
# Install dependencies
sudo apt-get install m4 tcsh csh libx11-dev tcl-dev tk-dev \
libcairo2-dev mesa-common-dev libglu1-mesa-dev libncurses-dev

# Clone Magic repo
git clone https://github.com/RTimothyEdwards/magic
cd magic

# Configure, build, install
./configure
make
sudo make install
```

✅ Verified with `magic -d XR`

---

## 🎉 Summary

* ✅ Environment setup complete
* ✅ All required tools installed & verified
* 🛠️ Workspace ready for **RTL-to-GDS design flow**

📂 **Repository**: `RTL2GDS_Alchemy`
👨‍💻 **Author**: *TheVoltageVikingRam*
📚 **Program**: VLSI System Design (VSD)

---

👉 Next step: **Week 1 – RTL Design & Simulation Kickoff** 🎬

---

Would you like me to also make a **compact version** of this README (less step-by-step, more concise) so you can use it as the **repo front page**, and keep the detailed one inside a `docs/week0.md` file?
