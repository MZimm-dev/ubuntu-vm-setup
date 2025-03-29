# 🖥️ Ubuntu Server VM mit SSH-Zugriff

## 📌 Projektziel

In diesem Projekt habe ich eine virtuelle Maschine mit Ubuntu Server 22.04 in VirtualBox eingerichtet. Ziel war es, grundlegende Kenntnisse im Umgang mit Linux und Netzwerkzugriff über SSH zu erwerben.

---

## 🔧 Voraussetzungen

- Windows 11 (Host-System)
- [VirtualBox](https://www.virtualbox.org/)
- [Ubuntu Server ISO](https://ubuntu.com/download/server)
- PuTTY (SSH-Client)

---

## 🛠️ Schritte

### 1. Ubuntu ISO herunterladen

Von der offiziellen Ubuntu-Webseite.

### 2. Neue VM in VirtualBox anlegen

- Typ: Linux (Ubuntu 64-bit)  
- RAM: 2048 MB  
- Speicher: Dynamisch, 20 GB  
- Netzwerk: NAT

![VM Einstellungen](screenshots/01-vm-erstellen.png)

### 3. Ubuntu Server installieren

- Benutzer: `marcel`  
- Hostname: `ubuntu-vm`  
- SSH direkt bei der Installation aktiviert

![Installation](screenshots/02-installation.png)

### 4. SSH-Zugriff testen

Mit PuTTY von Windows aus verbunden:

```bash
ssh marcel@192.168.0.101
