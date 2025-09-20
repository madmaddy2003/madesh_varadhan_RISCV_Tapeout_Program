# 🚀 Week 0: RISC‑V Reference SoC Tapeout Program – Foundation & Tool Setup

Welcome to my **RISC‑V Reference SoC Tapeout Program** repository!
Week 0 was all about **setting up the environment and essential open-source tools** for the upcoming RTL-to-GDS design journey.
The focus was on ensuring a **stable workspace** to handle synthesis, simulation, circuit analysis, and layout tasks.

---

## 🎯 System & Virtual Machine Setup

| Specification 💻        | Details 📋    |
| ----------------------- | ------------- |
| **Operating System 🐧** | Ubuntu 20.04+ |
| **RAM 💾**              | 8 GB          |
| **Storage 💿**          | 40 GB HDD     |
| **vCPUs ⚡**             | 4             |

💡 *This configuration ensures smooth performance for toolchains, synthesis, and simulation.*

---

## ⚙️ Tools Installed

The following open-source VLSI tools were installed & verified:

| Tool                             | Status     | Purpose             |
| -------------------------------- | ---------- | ------------------- |
| 🧠 **Yosys**                     | ✅ Completed | RTL Synthesis       |
| 📟 **Icarus Verilog (Iverilog)** | ✅ Completed | Verilog Simulation  |
| 📊 **GTKWave**                   | ✅ Completed | Waveform Debugging  |
| ⚡ **Ngspice**                    | ✅ Completed | Circuit Simulation  |
| 🎨 **Magic VLSI**                | ✅ Completed | Layout Design |

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
make config-gcc
make
sudo make install
```

✅ Verified with `yosys` command
<img width="871" height="656" alt="Screenshot 2025-09-20 212352" src="https://github.com/user-attachments/assets/4667c1d8-df42-4db1-bd14-ebdc5cbb77da" />

---

### 📟 Iverilog – Verilog Simulator

**Installation**

```bash
sudo apt-get update
sudo apt-get install iverilog
```

✅ Verified with `iverilog -v`
<img width="797" height="659" alt="Screenshot 2025-09-20 212752" src="https://github.com/user-attachments/assets/9a21cf7f-3cd6-484e-a5e1-2853ac594b46" />

---

### 📊 GTKWave – Waveform Viewer

**Installation**

```bash
sudo apt-get update
sudo apt-get install gtkwave
```

✅ Verified with `gtkwave`
<img width="1180" height="664" alt="Screenshot 2025-09-20 212940" src="https://github.com/user-attachments/assets/3071df8f-f7a0-48b1-9497-5e88373c9655" />

---

### ⚡ Ngspice – Circuit Simulator

**Installation**

```bash
sudo apt-get update
sudo apt-get install ngspice
```

✅ Verified with `ngspice -v`
<img width="809" height="242" alt="Screenshot 2025-09-20 213109" src="https://github.com/user-attachments/assets/835b0a83-b8d8-45f6-8340-b69f67deddda" />

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
<img width="1226" height="720" alt="Screenshot 2025-09-20 213256" src="https://github.com/user-attachments/assets/3bffbfa0-5ca6-4acb-860f-958456287d8c" />

---

## 🎉 Summary

* ✅ Environment setup complete
* ✅ All required tools installed & verified
* 🛠️ Workspace ready for **RTL-to-GDS design flow**

📂 **Repository**: `madesh_varadhan_RISCV_Tapeout_Program`
👨‍💻 **Author**: *madmaddy2003*
📚 **Program**: RISC‑V Reference SoC Tapeout Program

---

👉 Next step: **Week 1 – RTL Design & Simulation Kickoff** 🎬

---

Would you like me to also make a **compact version** of this README (less step-by-step, more concise) so you can use it as the **repo front page**, and keep the detailed one inside a `docs/week0.md` file?
