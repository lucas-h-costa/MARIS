<p align="center">
  <img src="MARIS.jpg" alt="MARIS Logo" width="130"/>
</p>

#  MARIS - Hydrographic & Navigation Data Simulator

**MARIS** is a desktop simulation suite designed for testing, validating, and operating hydrographic survey software, marine navigation systems, and onboard sensor integrations without requiring physical vessel hardware.

[![Latest Release](https://img.shields.io/github/v/release/lucas-h-costa/MARIS?label=Download%20Latest%20Release&style=for-the-badge)](https://github.com/lucas-h-costa/MARIS/releases/latest)

---

## 1 Key Capabilities

- **Multi-Sensor Telemetry Routing**:
  - Simulate an entire vessel instrument suite simultaneously across independent **Serial (`COM`)**, **UDP**, **TCP**, and **Local** channels, each with its own configurable transmission rate (`0.5 Hz` ? `10.0 Hz`).
  - Example setup: stream GNSS position over `COM5`, Gyro & Motion Reference Unit (MRU) over `UDP`, and Echo Sounder depth over `COM9` concurrently.
- **Wave, Attitude & Depth Generator**:
  - Synthesize realistic sea-state motion across **Pitch**, **Roll**, **Heave**, **Heading (Yaw)**, and **Depth**.
  - Choose between **Fixed**, **Sinusoidal** (with primary wave cycle and secondary swell envelope modulation), and **Course Made Good (`CMG`)** modes, or apply one-click sea-state presets (*Calm Sea* / *Moderate Swell*).
- **Interactive Navigation Map & Auto-Pilot**:
  - Visualize real-time vessel position, heading, wake trail, and survey/patrol routes on an interactive map.
  - Create waypoints directly on the map with a right-click, or import/export routes in `.csv`, `.json`, and `.gpx` formats.
  - Engage the **Auto-Pilot** to steer the vessel automatically along waypoint lines at a configurable cruise speed.
- **Instant Manual Overrides**:
  - Lock any vessel or environmental parameter (Speed, Heading, Pitch, Roll, Heave, Rate of Turn, Depth, Water Temperature, or Wind) on the fly using live sliders.
- **Built-In User Manual**:
  - Click **Help** inside the application at any time to open the complete, searchable User Manual with an interactive Table of Contents.

---

## 2 Supported NMEA 0183 Sentences (Strict UTC)

All time- and date-stamped sentences are generated strictly in **UTC**:

| Category | Supported Sentences |
| :--- | :--- |
| **GNSS & Timing** | `GGA`, `GLL`, `GSA`, `GSV`, `RMC`, `VTG`, `ZDA`, `MSS` |
| **Depth, Speed & Distance Log** | `DBT`, `DPT`, `DBS`, `MTW`, `VHW`, `VLW` |
| **Heading, Wind & Waypoints** | `HDT`, `ROT`, `MWV`, `BWC`, `WPL` |
| **Attitude & Hydrographic Motion** | `XDR` *(Pitch, Roll, Heave)*, `PASHR`, `PRDID` |

---

## 3 Download & Installation

1. Go to the [**Releases**](https://github.com/lucas-h-costa/MARIS/releases/latest) page.
2. Download the latest Windows installer (**`MARIS_Setup_v0.1.1.exe`**).
3. Run the installer and follow the on-screen setup wizard.
4. Launch **MARIS** from the Windows Start Menu or Desktop shortcut.

---

## 4 About & Contact

- **Current Version:** `0.1.1`
- **Release Date:** Sep. 29th, 2026
- **Author:** Lucas H. Costa
- **Contact:** [dacosta.lhm@gmail.com](mailto:dacosta.lhm@gmail.com)
