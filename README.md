# 🚀 Ubuntu Autoinstall Lab

<p align="center">
  <img src="https://img.shields.io/badge/Ubuntu-Autoinstall-E95420?logo=ubuntu&logoColor=white"/>
  <img src="https://img.shields.io/badge/Automation-Zero%20Touch-blue"/>
  <img src="https://img.shields.io/badge/Status-Development-yellow"/>
  <img src="https://img.shields.io/badge/License-MIT-green"/>
</p>

---

## 📌 Overview

This project focuses on **automating Ubuntu installations** using the `autoinstall` feature.

It is designed for:

- 💻 Virtual machine testing
- 🏢 Real-world infrastructure deployment
- ⚙️ Reproducible system provisioning

---

## 🎯 Goals

- Zero-touch installation
- Safe disk handling (multi-disk environments)
- Reliable network-based provisioning
- Automated software setup
- Reproducible environments

---

## 📂 Project Structure

```
.
├── examples/
│   ├── virtualbox.yaml
│   └── nitro5.yaml
└── README.md
```

---

## 🧪 Environments

### 🔹 VirtualBox (Testing)

File:
```
examples/virtualbox.yaml
```

Features:
- Simple storage layout
- Safe for testing
- Fast iteration

---

### 🔹 Production (Real Hardware)

File:
```
examples/nitro5.yaml
```

Features:
- Disk selection via SERIAL
- `/home` preservation
- Backup disk protection
- Full automation

---

## ⚙️ Features

- ✔ Automated Ubuntu installation
- ✔ Disk safety using serial matching
- ✔ Internet validation before install
- ✔ Retry mechanism for downloads
- ✔ Automatic package installation
- ✔ SSH enabled by default

---

## 🌐 Network Resilience

The setup includes:

- Retry logic (multiple attempts)
- DNS fallback
- Dependency auto-fix
- Connectivity checks before execution

---

## 📦 Software Provisioning

Includes automated installation of:

- Development tools
- Network utilities
- System tools
- Optional GUI applications

(Customizable via YAML)

---

## 🚀 Usage

1. Customize your YAML file
2. Inject into Ubuntu ISO (optional)
3. Boot system
4. Let autoinstall do the rest

---

## 🧪 Testing Workflow

1. Test in VirtualBox
2. Validate installation logs
3. Adjust configuration
4. Deploy to real hardware

---

## 🔍 Logs & Debugging

Useful logs:

```
/var/log/installer/
/var/log/cloud-init.log
/home/<user>/install.log
```

---

## ⚠️ Important Notes

- Always test before production
- Validate disk serials carefully
- Ensure internet connectivity
- Review YAML syntax

---

## 🧭 Roadmap

- [ ] Boot automation (no GRUB interaction)
- [ ] Offline ISO support
- [ ] PXE network installation
- [ ] LVM support
- [ ] Advanced hardware detection

---

## 🤝 Contributing

Contributions are welcome.

---

## 📄 License

MIT License

---

## 👨‍💻 Author

Ivan Junior  
Infrastructure | Networking | Automation
