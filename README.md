# 📊 Windows Server Monitoring Dashboard (WPF + PowerShell)

A custom-built desktop application for real-time monitoring of Windows Servers and Virtual Machines across hybrid environments. Built using **C# WPF** with backend integration via **PowerShell** and **WMI**, this tool provides system health visibility, alerting, and dynamic filtering in a clean, operator-friendly UI.

---

## 🧠 Purpose

To provide a centralized, lightweight, and extensible monitoring solution that tracks CPU, memory, uptime, disk usage, and system status for Windows-based infrastructure. Built for homelab, enterprise lab, or IT department use.

---

## 🛠️ Features

| Feature                       | Description                                           |
|------------------------------|-------------------------------------------------------|
| ✅ Dynamic Filters            | Filter by name, IP, VLAN, type, status, time updated |
| 🔄 Auto-Refresh               | Every 5 minutes, with manual refresh button          |
| 📊 Real-Time Metrics         | CPU, RAM, uptime, ping status, storage levels        |
| 🖥️ Color-Coded Health Status | Visual indicators for health alerts                  |
| 📬 Alerting                  | Pop-up notifications + optional email/MS Teams hooks |
| 🔐 Session Auth              | Prompts for credentials on launch, securely stored   |
| 📄 Paginated Data Grid       | Clean layout for 10–50 servers per page              |

---

## 🧰 Tech Stack

- **Frontend:** C# with WPF (.NET Framework)
- **Backend:** PowerShell for remote data collection (PSRemoting + WMI)
- **UI Charts:** LiveCharts
- **Security:** In-session credential storage, no persistent secrets

---

## 📁 Folder Structure

```bash
windows-server-monitoring/
├── src/
│   ├── MainWindow.xaml
│   ├── ServerModel.cs
│   ├── MonitoringLogic.cs
│   └── AlertService.cs
├── scripts/
│   ├── check-status.ps1
│   └── remote-wmi-query.ps1
├── docs/
│   ├── dashboard-screenshot.png
│   └── usage-guide.md
├── bin/
└── README.md
