# 699 Aura Checker 🔥

A modern hardware inspector with style. Check your PC's specs, get an "aura level" rating, and flex on your friends.

![Python](https://img.shields.io/badge/Python-3.8+-blue.svg)
![License](https://img.shields.io/badge/License-MIT-green.svg)
![Platform](https://img.shields.io/badge/Platform-Windows%20%7C%20macOS%20%7C%20Linux-lightgrey.svg)

## Features

- **Hardware Detection** — CPU, GPU, RAM, Storage, Battery
- **Aura Rating** — Score your rig from 1-10 with fun tier names
- **Live Monitoring** — Real-time CPU/RAM graphs and process list
- **CPU Benchmark** — SHA-256 hashing performance test
- **Network Info** — IP addresses and data usage
- **HTML Export** — Save styled reports
- **Rig Name Generator** — Random cool names for your PC

## Aura Levels

| Score | Aura | Meaning |
|-------|------|---------|
| 9-10 | ASCENDED | Legendary Tier |
| 7.5-9 | PEAK | Main Character Energy |
| 6-7.5 | SOLID | Vibes Intact |
| 4-6 | CHILL | Budget Build |
| 0-4 | GLITCH | Needs Upgrade |

## Installation

```bash
# Clone the repository
git clone https://github.com/yourusername/699-aura-checker.git
cd 699-aura-checker

# Run (dependencies auto-install)
python specs_aura_gui.py
```

### Manual Dependency Install

```bash
pip install PySide6 psutil GPUtil py-cpuinfo screeninfo distro qtawesome
```

### Linux Users

```bash
sudo apt install libxcb-cursor0
```

## Usage

```bash
# GUI Mode
python specs_aura_gui.py

# Headless Mode (terminal output)
python specs_aura_gui.py --headless
```

### Headless Output

```
==================================================
  699 AURA: 7.2/10
  PEAK - Main Character Energy
==================================================
  CPU: AMD Ryzen 7 5800X
       8 cores / 16 threads
  GPU: NVIDIA GeForce RTX 3070
  RAM: 32.0 GB
  Storage: 1000 GB SSD
==================================================
```

## Screenshots

| Overview | Monitor | Benchmark |
|----------|---------|-----------|
| Hardware cards, score ring, rig names | Live CPU/RAM charts, process table | Single/multi-thread testing |

## Tech Stack

- **GUI**: PySide6 (Qt6)
- **Icons**: QtAwesome (FontAwesome)
- **System Info**: psutil, GPUtil, py-cpuinfo
- **Charts**: Qt Charts

## How Scoring Works

```
Final Score = CPU (30%) + GPU (30%) + RAM (20%) + Storage (20%)

CPU Score:
  Base 3 + (cores × 0.5) + bonus for i9/Ryzen 9/M3/M4

GPU Score:
  Base 2 + (VRAM ÷ 2000) + RTX bonus

RAM Score:
  Base 2 + (GB ÷ 8)

Storage Score:
  Base 5 + SSD bonus (2) + (GB ÷ 500)
```

## License

MIT License - Do whatever you want with it.

## Contributing

PRs welcome! Open an issue first for major changes.

---

**Made with ❤️ for the culture**
