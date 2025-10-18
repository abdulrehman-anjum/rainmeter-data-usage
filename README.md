````markdown
# 📶 Rainmeter Data Usage Tracker

A minimal, lightweight Rainmeter skin that tracks your **real-time internet data usage (download & upload)** directly from your Wi-Fi interface.  
I built this because I couldn’t find any simple skin online that does exactly this — so here it is, for myself and anyone else who might find it useful.

---

## 🧠 Features

- Displays **live data usage (MB)** updated every second  
- Clean, minimal layout for seamless desktop integration  
- Built-in **Task Manager shortcut** (click the usage bar)  
- Fully customizable colors, fonts, and interface name  
- Very light on system resources

---

## 🧩 Requirements

- [Rainmeter](https://www.rainmeter.net/) (latest stable version)  
- Basic understanding of `.ini` files (for customization)  

---

## 🚀 Installation

1. Download or clone this repository:
   ```bash
   git clone https://github.com/abdulrehman-anjum/rainmeter-data-usage.git
````

2. Copy the folder into your **Documents\Rainmeter\Skins** directory.
3. Refresh Rainmeter and load the skin:

   * Right-click Rainmeter icon in the system tray
   * Choose **Skins → rainmeter-data-usage → DataUsage.ini**
4. You’re done. The skin should appear on your desktop showing your current network usage.

---

## ⚙️ Configuration

You can tweak a few settings in the `.ini` file to match your setup or style.

### 1. Network Interface

Make sure the skin is monitoring the correct network interface (Wi-Fi, Ethernet, etc.).
Open the `.ini` file and edit these lines:

```ini
Interface="Wi-Fi"
```

If you’re on Ethernet, change it to:

```ini
Interface="Ethernet"
```

Or find your exact adapter name in Rainmeter’s **Network measures** documentation.

### 2. Fonts

You can change the font names and sizes in the `[Variables]` section:

```ini
FontName=GeosansLight
FontName2=Segoe WP Semibold
FontSize=10
```

### 3. Colors

Modify text opacity or color using RGBA values:

```ini
FontColor=255,255,255,220
FontColor2=255,255,255,140
```

### 4. Background Position & Size

Adjust the background meters if needed:

```ini
[BG]
X=45
H=20
W=70

[BG2]
X=0
H=18
W=45
```

---

## 🖱️ Quick Tip

* **Left-click** the skin to open **Task Manager** instantly.

---

## 📂 Files Included

* `DataUsage.ini` — the main Rainmeter skin file
* `DataUsage.lua` — the Lua script for calculating total usage
* (Optional) supporting assets (if any in `@Resources` folder)

---

## 💡 Notes

* Updates every 1 second (`Update=1000`).
* The Lua script keeps cumulative data usage running while Rainmeter is active.
* Designed for simplicity — no unnecessary widgets or visual clutter.

---

## 🧑‍💻 Author

**Abdul Rehman Anjum**
[GitHub Repository](https://github.com/abdulrehman-anjum/rainmeter-data-usage)

---

## 🪶 License

This skin is open for personal use and modification.
If you re-upload or remix it, please credit the original creator.

---

> “Sometimes, if you can’t find the tool you need, you just build it yourself.”

```
```
