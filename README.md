.NET backend developer. On the side I build **transparent PowerShell alternatives** to closed-source Windows tweaking tools — every script fits on one screen, needs no install, and writes a `.reg` / backup undo before touching anything. They pair with [RigPolice](https://rigpolice.com/?utm_source=github&utm_medium=readme&utm_campaign=vadyaravadim), my site of free browser tests for gaming gear.

## Latency toolbox

<p align="center">
  <img src="assets/header.svg" alt="Vadim Cheban — .NET developer. Frame-time chart in a PowerShell window: 6.4 ms average before tweaks, 0.5 ms after." width="100%">
</p>

| Tool<img width="280" height="1"> | Replaces<img width="180" height="1"> | What it does<img width="290" height="1"> |
|:-----|:---------|:-------------|
| [cpu-parking-disabler](https://github.com/vadyaravadim/cpu-parking-disabler) <img align="right" src="https://img.shields.io/github/stars/vadyaravadim/cpu-parking-disabler?style=flat-square&label=%E2%98%85&labelColor=0A1F44&color=1B3A6B"> | ParkControl, Quick CPU | Unpark all CPU cores |
| [msi-mode-utility](https://github.com/vadyaravadim/msi-mode-utility) <img align="right" src="https://img.shields.io/github/stars/vadyaravadim/msi-mode-utility?style=flat-square&label=%E2%98%85&labelColor=0A1F44&color=1B3A6B"> | MSI Util v3 | MSI mode for GPU, USB, network, audio |
| [timer-resolution-utility](https://github.com/vadyaravadim/timer-resolution-utility) <img align="right" src="https://img.shields.io/github/stars/vadyaravadim/timer-resolution-utility?style=flat-square&label=%E2%98%85&labelColor=0A1F44&color=1B3A6B"> | TimerResolution.exe, ISLC | 0.5 ms timer + `Sleep(1)` benchmark |
| [interrupt-affinity-utility](https://github.com/vadyaravadim/interrupt-affinity-utility) <img align="right" src="https://img.shields.io/github/stars/vadyaravadim/interrupt-affinity-utility?style=flat-square&label=%E2%98%85&labelColor=0A1F44&color=1B3A6B"> | GoInterruptPolicy | Pin interrupts to cores, P/E-aware |
| [gamedvr-fso-disabler](https://github.com/vadyaravadim/gamedvr-fso-disabler) <img align="right" src="https://img.shields.io/github/stars/vadyaravadim/gamedvr-fso-disabler?style=flat-square&label=%E2%98%85&labelColor=0A1F44&color=1B3A6B"> | — | Disable Game DVR &amp; FSO |
| [remove-hidden-devices](https://github.com/vadyaravadim/remove-hidden-devices) <img align="right" src="https://img.shields.io/github/stars/vadyaravadim/remove-hidden-devices?style=flat-square&label=%E2%98%85&labelColor=0A1F44&color=1B3A6B"> | — | Remove ghost devices from Device Manager |

Every tool follows the same contract: read the script before you run it, undo file written before any change, one command to apply.

## Check the result

A tweak is worth keeping only if you can measure it. These free browser tests on RigPolice pair with the tools above:

- After MSI mode or interrupt affinity: [Mouse Polling Rate Test](https://rigpolice.com/mouse/tests/polling-rate-test/?utm_source=github&utm_medium=readme&utm_campaign=vadyaravadim)
- After a timer resolution change: [Refresh Rate Test](https://rigpolice.com/monitor/tests/refresh-rate-test/?utm_source=github&utm_medium=readme&utm_campaign=vadyaravadim)
- After a ghost device cleanup: [Mouse Test](https://rigpolice.com/mouse/tests/mouse-test/?utm_source=github&utm_medium=readme&utm_campaign=vadyaravadim)
- Before you unpark cores: [How to Disable CPU Core Parking in Windows 11, and Whether It Helps](https://rigpolice.com/system/articles/disable-cpu-core-parking/?utm_source=github&utm_medium=readme&utm_campaign=vadyaravadim)

Also: [rigpolice-embed](https://github.com/vadyaravadim/rigpolice-embed), a zero-build WordPress block that embeds the RigPolice tests on any site.
