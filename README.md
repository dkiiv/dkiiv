### Curtis Jenkins

I'm a site reliability and systems engineer in Vancouver, WA. Day job: final escalation point for infrastructure and application incidents at WebMD Health Services. Outside of that I write firmware, poke at CAN buses, and reverse-engineer car ECUs in Ghidra.

**[4xavior.com](https://4xavior.com)** · [resume (PDF)](https://4xavior.com/resume/curtis-jenkins.pdf) · [LinkedIn](https://www.linkedin.com/in/curtis-jenkins-17b122153)

#### Start here

- **[Remote PC for Steam Frame](https://github.com/dkiiv/frametop/tree/remote-display-poc-handoff/remote-display)**: your Windows PC's monitors as panels inside the Steam Frame. A Moonlight client on the headset decodes in hardware and hands frames to the compositor as a zero-copy Wayland window. 13 ms median from input to decoded frame over Valve's USB adapter. Personal POC, works day to day on my setup.
- **[hermes-cf-access-sso](https://github.com/dkiiv/hermes-cf-access-sso)**: a Hermes Agent plugin that logs you in to the Hermes dashboard with your Cloudflare Access identity, so there is no second password. The Access token has to pass signature, issuer, audience, expiry and email allowlist checks before it counts, and the password stays as a LAN fallback. Offline tests in CI against Hermes v0.22.5, threat model in the README.
- **[docs-rag-mcp](https://github.com/dkiiv/docs-rag-mcp)**: semantic search and cited answers over markdown docs, served to Hermes over MCP on my local GPUs (bge-m3 plus a local chat model). On the Hermes docs, the right file was in the top 10 results for 95% of 40 generated questions. The README lists the caveats.
- **[ParkPlay](https://github.com/dkiiv/parkPlay)**: a YouTube player for the Tesla in-car browser. The browser pauses `<video>` in Drive, so the page decodes H.264/AAC itself with WebCodecs and draws to a canvas.
- **[deskBot](https://github.com/dkiiv/deskBot)**: motion and safety firmware for a motorized desk. The core compiles for the host and runs against a simulator in CI before it ever touches an ESP32.
- **[ocelot](https://github.com/dkiiv/ocelot)** and **[openpilot](https://github.com/dkiiv/openpilot/tree/sp_master_pla)**: STM32 steering firmware for older Volkswagens, built on [reverse-engineering the steering rack's V850 firmware](https://github.com/dkiiv/1K0909144-FW-Project).
- **[tesla-autoWiper](https://github.com/dkiiv/tesla-autoWiper)**: an ESP32 inline on a Tesla's CAN bus reading a VW rain sensor over LIN. Work in progress, not tested in a car yet. The README says so.

#### Merged upstream

[commaai/openpilot #31895](https://github.com/commaai/openpilot/pull/31895) ·
[commaai/opendbc #1208](https://github.com/commaai/opendbc/pull/1208) ·
[commaai/opendbc #3184](https://github.com/commaai/opendbc/pull/3184) ·
[sunnypilot #155](https://github.com/sunnypilot/sunnypilot/pull/155) ·
[MarlinFirmware/Marlin #19784](https://github.com/MarlinFirmware/Marlin/pull/19784) ·
[ArduinoAirSuspensionController #181](https://github.com/gopro2027/ArduinoAirSuspensionController/pull/181) ·
[Frametop #45](https://github.com/Frametop/frametop/pull/45)

#### Also

A homelab I run like production. One Proxmox host, three V100s doing local LLM inference (benchmarked from about 23 to about 100 tok/s), and zero inbound ports at home. Public services come in over Cloudflare Tunnels and WireGuard. Write-up and an interactive diagram on [4xavior.com](https://4xavior.com/#lab).
