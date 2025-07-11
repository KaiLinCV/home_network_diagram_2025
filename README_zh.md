📘 [English](README.md) | 📙 [中文](README_zh.md)

# 🏠 家用網路圖表 – 2025年6月

![NetworkDiagram](./img/NetworkDiagram.png)

這份圖表展示了我目前的家用網路與工作環境設定。我的目標是模擬一個小型辦公室／家庭辦公室(SOHO)環境，並建立一個家庭實驗室，進行系統管理相關任務的測試，監控與管理。

## 🧑‍💻 網路概述

我的家庭網路由有線與無線裝置組成，透過ASUS Wi-Fi路由器進行管理，並啟用內建防火牆功能。ASUS路由器透過由ISP提供的TP-Link Gigabit乙太網路媒體轉換器連接到光纖網路。第二台D-Link Wi-Fi路由器則用於實驗室網路隔離，提升安全性並支援封閉測試環境。

### 🔌 有線架構
- **PC 1 – Windows 11 Pro**  
  主要工作電腦，用於日常操作，系統設定，以及執行 Linux 虛擬機（如 Ubuntu Server，CentOS 9）進行測試。
- **PC 2 – Windows 10 Home（雙系統含 Linux）**  
  連接至D-Link路由器，用於 Linux 測試，作業系統設定與跨網段實驗。
- **Synology DS224+ NAS** 
  作為檔案備份，資料冗餘與集中式儲存設備，使用 SMB／AFP 協定管理。

### 🖥️ 周邊與顯示設備管理
- **2埠KVM切換器**  
  用於在兩台電腦之間共用鍵盤、滑鼠與雙螢幕顯示。KVM切換器讓我能在不同工作機之間快速切換以進行實驗與練習。
- **USB 集線器、外接硬碟（Seagate）**  
  擴充I/O用於備份作業與檔案管理。

### 🛜 無線裝置
- **MacBook Air、iPhone**  
  主要為個人使用設備，也可用於連線測試，VPN與跨平台遠端同步。
- **智慧電視、喇叭、PS4**  
  為日常娛樂用途的消費型裝置，雖非實驗重點，但可作為網路可見性，頻寬分配或分段測試的參考對象。

## 🔐 網路服務與安全性
- **ASUS 路由器（主要）** – 啟用SPI／NAT防火牆與DHCP
- **D-Link 路由器（次要）** – 實驗室網路隔離，具備獨立防火牆
- **DHCP 伺服器** – 提供內部IP配置
- **靜態 IP 對應** – 為NAS與虛擬機指定固定IP
- **虛擬機測試** – 使用VirtualBox部署Linux虛擬機，進行修補測試，自動化腳本與網段隔離實驗

---

### 結論

建立這套網路環境的目的，是為了實作系統管理的核心技能。這包括透過路由器分段設計網路架構，跨平台系統配置，防火牆與DHCP設定，NAS和KVM 等共用資源管理，以及周邊設備的整合。此環境支援透過隔離網段進行的實驗，虛擬機部署，修補測試，基礎服務架設(如SMB)與系統強化。這些配置幫助我更深入了解網路基礎，並透過實際操作模擬企業級系統管理的工作環境。
