> [!NOTE]
> We use GitHub to track bugs, discuss feature requests, and release executables.
> SafeFanControl is **not** open-source software.

<div align="center">

**English** | [简体中文](README.zh-Hans.md) | [繁體中文](README.zh-Hant.md) | [日本語](README.ja.md) | [한국어](README.ko.md) | [Deutsch](README.de.md) | [Español](README.es.md) | [Français](README.fr.md) | [Русский](README.ru.md)

</div>

---

# SafeFanControl

**Take Control of Your Mac's Fans**

SafeFanControl is a **native macOS app** that lets you monitor temperatures and manage fan speeds on Apple Silicon and Intel Macs. Free to download — your fans, your rules, and the system always gets them back if anything goes wrong.

[Download for macOS](https://github.com/SafeFanControl/SafeFanControl/releases)

---

## Features

### All the Fan Control Modes You May Need

SafeFanControl gives you complete control over how your Mac responds to heat, with three distinct operating modes to match your workflow.

- **Monitor** — read live temperatures and fan speeds without touching system control
- **Safe Max** — automatically ramp to full speed when a temperature threshold is hit, then return control to macOS when it cools down
- **Curve** — define a custom temperature-to-speed curve for continuous proportional control
- Switch modes instantly from the menu bar — no app window required

### Designed for Safety First

A three-process architecture ensures that if anything goes wrong, macOS always gets fan control back automatically — with no manual intervention needed.

- **Watchdog process** monitors the helper daemon; if it crashes while fans are in manual mode, macOS takes over instantly
- **Smooth fade transitions** prevent abrupt fan speed jumps that could be audible or disruptive
- **Threshold latching** keeps Safe Max stable during brief temperature fluctuations
- Standard macOS admin prompt installs the background helper — no Terminal, no manual steps

### Always in the Menu Bar

A lightweight menu bar app puts live sensor data and mode switching one click away — always visible, never in the way.

- Live CPU and GPU temperatures updated in real time
- Current fan speed and active control mode always visible
- Switch between Monitor, Safe Max, and Curve directly from the dropdown
- Supports M1 through M5 Apple Silicon and Intel T2 Macs; available in 8 languages

---

## Pricing

SafeFanControl follows a **free download, one-time purchase** model. No subscriptions. No recurring fees. Pay once, own it forever.

| | Free | Full License |
|---|---|---|
| **Price** | $0 — forever | $8.99 — one-time |
| Monitor mode (read-only) | ✅ | ✅ |
| Live temperature display | ✅ | ✅ |
| Fan speed display | ✅ | ✅ |
| CPU, GPU, SoC sensors | ✅ | ✅ |
| M1–M5 generation-aware | ✅ | ✅ |
| **Safe Max mode** | ❌ | ✅ |
| **Curve mode** | ❌ | ✅ |
| Smooth fade transitions | ❌ | ✅ |
| Latch / no-bounce logic | ❌ | ✅ |
| Multi-rule Safe Max | ❌ | ✅ |
| **Fan test wizard** | ❌ | ✅ |
| Debug & diagnostics page | ❌ | ✅ |

---

## Download & Install

### System Requirements

| Requirement | Details |
|---|---|
| **macOS** | 15 (Sequoia) or later |
| **Mac hardware** | Apple Silicon (M1, M2, M3, M4, M5) or Intel Mac with T2 chip |
| **Permissions** | One admin password prompt to install the background helper daemon |
| **Disk space** | ~5 MB |

### Installation

1. **Open the downloaded `.dmg`** and drag SafeFanControl to your Applications folder.
2. **Launch the app.** On first run, an admin dialog installs the background helper and watchdog daemons.
3. **Done.** No Terminal. No manual approvals. The Fan Test Wizard will guide you through confirming everything works on your hardware.

> macOS may show a Gatekeeper prompt on first launch since the app is not App Store distributed. **Right-click → Open** to proceed.

### Uninstall

SafeFanControl includes a complete uninstall flow in **Settings → Uninstall**. It removes the helper daemon, watchdog daemon, and all associated files in one step.

---

## FAQ

**Is there a free trial for the full features?**
Yes — Safe Max and Curve modes are unlocked for a **14-day trial** upon first launch. No payment required.

**What does the license cover?**
One license covers all your **personal** Macs. It is not for redistribution or commercial fleet use.

**Do I need to re-purchase after a macOS upgrade?**
No. Your license is permanent.

**Do I need to re-purchase if I get a new Mac?**
No — your license belongs to you. Use your existing license key to register on your new Mac.

**What is your refund policy?**
Because we respect your privacy, the app uses an offline registration system. Once a license key is issued, it cannot be remotely deactivated — therefore all sales are final and standard refunds cannot be issued. We strongly encourage you to use the 14-day trial before purchasing. Exception: if an Apple macOS update permanently disables the underlying fan control methods, we will issue a full refund for licenses purchased within the last 30 days.

**Why isn't the app on the Mac App Store?**
SafeFanControl installs a privileged background helper daemon, which is incompatible with the App Store's strict sandboxing rules. Distribution is direct — but the installer is scanned, notarized, and signed through Apple's signing system.

**Can I use it without paying?**
Yes — Monitor mode is completely free and always will be.

**What happens if the licensing server goes offline in the future?**
The license key works offline and does not require an internet check. You can register at any time, as long as you still have your license key.

**What if you abandon this project?**
Every product has a lifespan. However, as long as I am able to code and the product's revenue covers its basic expenses (such as the yearly Apple Developer Program fee), I will continue maintaining it. If you like this product, please share it with your friends. If (and only if) the day comes when I have to abandon this project, I will share the source code with all paid users under the AGPL v3 license.

**What if I lose my license key?**
Please reach out to the vendor platform or contact us directly.

---

## Privacy

SafeFanControl does **not** collect telemetry, analytics, or crash reports. Your hardware data stays on your device.
