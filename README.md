<div align="center">

# Zaid Ahmad

CS @ Carleton University &nbsp;·&nbsp; Ottawa, Canada

[![Portfolio](https://img.shields.io/badge/zaidahmad.dev-000?style=flat-square&logo=safari&logoColor=white)](https://zaidahmad.dev)&nbsp;
[![LinkedIn](https://img.shields.io/badge/LinkedIn-0a66c2?style=flat-square&logo=linkedin&logoColor=white)](https://linkedin.com/in/zaid-ahmad-ba9b10224)&nbsp;
[![Email](https://img.shields.io/badge/Email-ea4335?style=flat-square&logo=gmail&logoColor=white)](mailto:zaidahmad8060@gmail.com)

</div>

<br/>

CS student at Carleton building across the full depth of the stack — Linux kernel patches, bare-metal firmware on Cortex-M4, and deployed web apps. Drawn to problems where the constraints are physical: clock cycles, memory layouts, hardware registers.

Open to internships in systems, embedded, or full-stack engineering.

<br/>

---

### Skills

**Languages**

<img src="https://skillicons.dev/icons?i=c,cpp,python,js,ts,java&theme=dark" />

**Web & Tooling**

<img src="https://skillicons.dev/icons?i=linux,git,nodejs,react,nextjs,firebase,mongodb,postgresql,supabase,neon,tailwind,githubactions&theme=dark" />

**Embedded & Systems**

`STM32` `ARM Cortex-M4` `POSIX Threads` `DKMS` `devkitARM`

---

### Projects

**[mac80211-ht-downgrade-fix](https://github.com/zaidahmad16/mac80211-ht-downgrade-fix)**

Linux kernel patch fixing a Wi-Fi 6 throughput regression. Malformed HT Operation beacons from certain routers cause `mac80211` to fall back to legacy 802.11g speeds. A single targeted fix to `mlme.c` — mirroring validation already present in the VHT codepath — restores full throughput without breaking compatibility. Ships via DKMS; rebuilds automatically on kernel updates. **54 Mbps → 1036 Mbps on affected hardware.**

`C` `Linux Kernel` `mac80211` `DKMS`

<br/>

**[stm32-doom-loader](https://github.com/zaidahmad16/stm32-doom-loader)**

Bare-metal bootloader for the STM32F401RE — the foundation for eventually running Doom on a microcontroller. No HAL, no RTOS. Custom linker script, hand-written startup assembly, CRC32 verification of staged application images before jump-to-execution. A Python utility pads and footers the binary; a bad checksum traps instead of running corrupt code. ILI9341 display driver and SD card interface in progress.

`C` `STM32` `ARM Cortex-M4` `Bare-Metal` `Python`

<br/>

**[DS Business Card](https://github.com/zaidahmad16/DS_Business_Card)**

Nintendo DS homebrew that doubles as an interactive business card. The top screen runs a live step-by-step Counting Sort visualization at 60 FPS via VBlank sync; the bottom screen renders a static contact card. Direct VRAM writes and DMA transfers keep the rendering pipeline off the CPU. Cross-compiled for the ARM9 with devkitARM; validated on real hardware (Nintendo 3DS XL).

`C` `devkitARM` `libnds` `ARM9` `DMA`

<br/>

**[CarletonCourseMap](https://github.com/zaidahmad16/CarletonCourseMap)**

Web app for exploring Carleton University's full course catalog interactively. A Python scraper pulls and normalizes course data from Carleton's systems into a structured dataset; a JavaScript frontend surfaces it cleanly. Deployed on Vercel and live at [carletoncoursemap.ca](https://carletoncoursemap.ca).

`Python` `JavaScript` `Web Scraping` `Vercel`

<br/>

**[COMP2401 — Multithreaded Simulation](https://github.com/zaidahmad16/COMP2401-Final-Project)**

Concurrent ghost-hunt simulation in C. Hunters and a ghost move through a 13-room building on independent POSIX threads. Semaphores protect shared state; deadlock prevention uses ordered mutex acquisition across room addresses. Hunters collect bitwise-matched evidence while fear and boredom thresholds drive emergent behavior. Pure C — no external libraries.

`C` `POSIX Threads` `Semaphores` `Systems Programming`

<br/>

**[Suburban Street Brawl](https://github.com/vinit-rao/SuburbanStreetBrawlUnity)**

Collaborative 2D brawler in Unity. Combat mechanics, physics-driven movement, level design. Active development.

`C#` `Unity`

---

<br/>

<div align="center">

![GitHub Stats](https://github-readme-stats.vercel.app/api?username=zaidahmad16&show_icons=true&theme=github_dark&hide_border=true&title_color=ffffff&text_color=888888&icon_color=4493f8&bg_color=0d1117)&nbsp;
![Top Languages](https://github-readme-stats.vercel.app/api/top-langs/?username=zaidahmad16&layout=compact&theme=github_dark&hide_border=true&title_color=ffffff&text_color=888888&bg_color=0d1117)

</div>
