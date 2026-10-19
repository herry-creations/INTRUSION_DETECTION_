# INTRUSION_DETECTION_
A professional desktop IDS built with Python, CustomTkinter, and Scapy for real-time packet monitoring and alerting.  Intrudex 🔐

A professional Python-based Intrusion Detection System (IDS) with a modern GUI, real-time packet monitoring, interface selection, and log export support.

Overview 📌

Intrudex is a desktop network monitoring tool built with Python, CustomTkinter, and Scapy. It captures live TCP traffic, detects basic suspicious patterns, and displays alerts in a clean dashboard-style interface.

This project was developed as a final project for information security coursework.

Features ✨

Modern dark-themed GUI 🌙

Real-time packet sniffing using Scapy 📡

Friendly interface selection for Windows adapters 🖧

Automatic mapping of Windows NPF devices to readable names 🪟

Live alert dashboard 📊

Uptime counter ⏱️

Save logs to JSON 💾

Custom app icon support 🖼️

Tech Stack 🛠️

Python 3.14+
CustomTkinter
Scapy
Tkinter
PyInstaller for packaging
How It Works ⚙️

Intrudex monitors selected network traffic and applies simple detection rules:

SYN packets are flagged as potential scan activity ⚠️

SSH traffic is highlighted 🔒

HTTP/HTTPS traffic is tracked 🌐

All captured alerts are shown in real time and can be saved to a JSON file 📝

Installation 📦


Install dependencies

pip install customtkinter scapy pyinstaller

Install Npcap Scapy on Windows requires Npcap for packet capture.

Download and install Npcap, then restart your system.

Running the Project 🚀

Run from Python

python ids.py
Build EXE with PyInstaller

pyinstaller --onefile --noconsole --name Intrudex --icon=intrudex.ico --add-data "intrudex.ico;." ids.py

The final executable will be created inside the dist folder.

Usage 🧭

Open the application.

Select the correct network interface from the dropdown.

Click Start Monitoring.

Generate traffic on your network.

View live alerts in the log panel.

Click Stop Monitoring when finished.

Save logs using the save button or Ctrl+S.

Project Structure 🗂️

.
├── ids.py
├── intrudex.ico
├── README.md
└── security_logs.json
Notes 📝

Run the application as Administrator for proper packet capture on Windows.
If no packets appear, try another interface from the dropdown.
The interface names are mapped automatically from Windows NPF adapters.
Screenshots 🖼️

Add screenshots here if available.
<img width="1363" height="704" alt="image" src="https://github.com/user-attachments/assets/5bbabf1b-876a-4a23-92ff-17fff7abe1da" />
<img width="1367" height="707" alt="image" src="https://github.com/user-attachments/assets/64754646-0aac-4b6d-bc42-52d72ad307f5" />
<img width="1372" height="701" alt="image" src="https://github.com/user-attachments/assets/e35b3e51-aa11-4db6-a584-833c8fdde857" />
Future Improvements 🔮

Advanced anomaly detection.
IP blocking support.
Live statistics charts.
Export to CSV and PDF.
Better rule engine.
License 📄

This project is for educational purposes.
