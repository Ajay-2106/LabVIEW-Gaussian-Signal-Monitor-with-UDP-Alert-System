
It continuously monitors the signal, and when the value crosses a user-defined threshold, the relevant data is transmitted over UDP. Simultaneously, the waveform and the crossing points are plotted on the front panel for real-time visualization.

## 🎯 Features

- **Signal Generation**: Real-time Gaussian waveform using `x(t) = exp(-(t - k)^2)`
- **Threshold Detection**: User-defined threshold for crossing detection
- **UDP Communication**: Sends data packets over UDP when the threshold is crossed
- **Live Plotting**: Front panel shows the full waveform and highlights threshold-crossing points

## 📦 Project Includes

- LabVIEW VI files
- UDP configuration settings
- Real-time graph with highlighted threshold events

## 🧪 How It Works

1. Gaussian signal is generated with tunable parameter `k`.
2. Each value is compared against a defined threshold.
3. If a value exceeds the threshold:
   - A UDP message is sent containing the timestamp and value.
   - The value is plotted distinctly on the front panel graph.
4. The signal and threshold events are continuously visualized.

## 🔧 Requirements

- NI LabVIEW (2018 or later recommended)
- UDP-capable network setup (localhost or remote)
- Basic familiarity with LabVIEW front panel and block diagram

## 📈 Example Use Case

This tool is useful for simulating sensor-like behavior where threshold breaches trigger network-based alerts — such as in anomaly detection, early warning systems, or real-time monitoring prototypes.
