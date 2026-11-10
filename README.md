### Curtis Jenkins

Site reliability and systems engineer in Vancouver, WA. My day job is keeping production up: I'm the final escalation point for infrastructure and application incidents at WebMD Health Services. When the problem sits below the operating system, I go down to the metal: C firmware, CAN/LIN buses, Ghidra.

**[4xavior.com](https://4xavior.com)** · [résumé (PDF)](https://4xavior.com/resume/curtis-jenkins.pdf) · [LinkedIn](https://www.linkedin.com/in/curtis-jenkins-17b122153)

#### Start here

- **[Remote PC for Steam Frame](https://github.com/dkiiv/frametop/tree/remote-display-poc-handoff/remote-display)**: a Windows PC's monitors as panels inside the Steam Frame. A Moonlight client on the headset decodes in hardware and hands frames to the compositor as a zero-copy Wayland window. Input to decoded frame is 13 ms median over Valve's USB adapter. Personal POC.
- **[ParkPlay](https://github.com/dkiiv/parkPlay)**: a YouTube player for the Tesla in-car browser, which suspends `<video>` in Drive. The page decodes H.264/AAC itself with WebCodecs and paints to a canvas.
- **[deskBot](https://github.com/dkiiv/deskBot)**: motion and safety firmware for a motorized desk. The core is host-compiled and runs against a simulator in CI before it touches an ESP32.
- **[ocelot](https://github.com/dkiiv/ocelot)** and **[openpilot](https://github.com/dkiiv/openpilot/tree/sp_master_pla)**: STM32 steering firmware for legacy Volkswagens, built from [reverse-engineering the steering rack's V850 firmware](https://github.com/dkiiv/1K0909144-FW-Project).
- **[tesla-autoWiper](https://github.com/dkiiv/tesla-autoWiper)**: an ESP32 inline on a Tesla's CAN bus, reading a rain sensor over LIN. Work in progress and not yet tested in a car; the README says so.

#### Merged upstream

[commaai/openpilot #31895](https://github.com/commaai/openpilot/pull/31895) ·
[commaai/opendbc #1208](https://github.com/commaai/opendbc/pull/1208) ·
[commaai/opendbc #3184](https://github.com/commaai/opendbc/pull/3184) ·
[sunnypilot #155](https://github.com/sunnypilot/sunnypilot/pull/155) ·
[MarlinFirmware/Marlin #19784](https://github.com/MarlinFirmware/Marlin/pull/19784) ·
[ArduinoAirSuspensionController #181](https://github.com/gopro2027/ArduinoAirSuspensionController/pull/181) ·
[Frametop #45](https://github.com/Frametop/frametop/pull/45)

#### Also

A homelab I run like production: one Proxmox host, three V100s doing local LLM inference (benchmarked from ~23 to ~100 tok/s), and zero inbound ports at home. Public services come in over Cloudflare Tunnels and WireGuard. The write-up and an interactive diagram are on [4xavior.com](https://4xavior.com/#lab).
