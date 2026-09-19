<div align="center">

# Zaid Ahmad

<sub>Carleton University · CS, AI/ML stream · Ottawa, Canada</sub>

[![Portfolio](https://img.shields.io/badge/zaidahmad.dev-000?style=flat-square&logo=safari&logoColor=white)](https://zaidahmad.dev)&nbsp;
[![LinkedIn](https://img.shields.io/badge/LinkedIn-0a66c2?style=flat-square&logo=linkedin&logoColor=white)](https://linkedin.com/in/zaid-ahmad-ba9b10224)&nbsp;
[![Email](https://img.shields.io/badge/Email-ea4335?style=flat-square&logo=gmail&logoColor=white)](mailto:zaidahmad8060@gmail.com)

</div>

<br/>

```
[    0.000000] zaid-ahmad: booting personality v2024.09 (Carleton-CS, AI/ML stream)
[    0.000142] kernel: minor in mathematics detected, enabling proofs subsystem
[    0.041223] curiosity: init OK — default policy: "understand it from the metal up"
[    1.402911] mac80211: throughput anomaly found (54 Mbps, expected 1000 Mbps)
[    1.402955] mac80211: root-caused in-stack, patch written, upstream-worthy — FIXED
[    2.881023] stm32f4_bootloader: no HAL, no engine, bare-metal SPI — loading DOOM.WAD
[    2.998117] stm32f4_bootloader: [ OK ] shareware doom booted from SD card
[    4.550012] ontariodrivetestmap: every public source traces to one fabricated route
[    4.550098] ontariodrivetestmap: building real corroboration pipeline — IN PROGRESS
[    5.001887] carletoncoursemap: 1700+ students mounted, serving read-write
[    5.998221] rpi_packet_analyzer: raw AF_PACKET capture online, <100MB on Pi 5
[    6.500000] ghost_hunting_sim: 1000+ ticks, 0 deadlocks — thread-safety: PROVEN
[  ready ]
zaid-ahmad login: _
```

<br/>

### `whoami`

I like understanding things from the metal up. Most of what's below started with "how does this actually work" — a Wi-Fi card silently capped at 5% of its real speed, a business card that's just a business card, a province full of driving-test routes nobody's ever independently verified. B.Sc. Computer Science at Carleton, AI & Machine Learning stream, minor in math.

<br/>

### `cat /proc/status`

```
currently_building  : OntarioDriveTestMap — real corroborated Ontario driving-test routes
currently_learning  : whatever the next project demands
last_bug_fixed      : mac80211 driver capping Wi-Fi at 54 Mbps instead of 1 Gbps
grad_year           : 2029
```

---

### `mount /projects`

**[Carleton Course Map](https://carletoncoursemap.ca/map)** &nbsp;·&nbsp; [source](https://github.com/zaidahmad16/CarletonCourseMap) &nbsp;·&nbsp; `[ OK ]` serving 1,700+ students

My program didn't have a course map, so people were planning entire degrees by reading prerequisite text course-by-course. Scraped Carleton Central, modelled AND/OR prerequisite logic as a DAG, designed a normalized 8-table Postgres schema, and shipped a rate-limited FastAPI backend behind a drag-and-drop Next.js planner.

`Python` `Parsel/XPath` `FastAPI` `PostgreSQL` `Next.js` `React Flow` `dagre`

<br/>

**[OntarioDriveTestMap](https://github.com/zaidahmad16/OntarioDriveTestMap)** &nbsp;·&nbsp; `[ IN PROGRESS ]`

Every major public source for Ontario driving-test routes traces back to the same fabricated route, repeated across every competitor. Building a real corroboration pipeline instead — independent YouTube dashcam footage and Reddit accounts, OCR/ASR turn extraction, snapped to the real OSM road graph, clustered with HDBSCAN into a confidence-weighted route graph. Splitting G/G2 consensus separately instead of pooling them raised edge-level F1 from 0.79 to 0.86.

`Python` `YouTube Data API` `PaddleOCR` `OSRM` `HDBSCAN` `PostgreSQL/PostGIS` `Next.js` `MapLibre GL JS`

<br/>

**[RPi Network Packet Analyzer](https://github.com/zaidahmad16/rpi-packet-analyzer)** &nbsp;·&nbsp; `[ OK ]` <100MB resident on a Pi 5

Wanted real frame-level traffic analysis, which ruled out higher-level capture libraries. Wrote a real-time engine in C on raw `AF_PACKET` sockets, hand-parsing Ethernet/IP/TCP/UDP headers and tracking per-source traffic with a hash map + min-heap top-K. Fixed thresholds kept flagging normal traffic as suspicious, so I trained a scikit-learn Isolation Forest on the captured features instead, exposed through Prometheus to a Grafana dashboard.

`C` `Python` `scikit-learn` `Raw Sockets` `Prometheus` `Grafana` `AWS`

<br/>

**[STM32 Doom Bootloader](https://github.com/zaidahmad16/stm32-doom-loader)** &nbsp;·&nbsp; `[ OK ]` boots real hardware

I wanted to understand how something actually boots, so I wrote a bootloader from scratch. No HAL, no game engine — bare-metal SPI on an STM32F4 loading shareware Doom off an SD card.

`C` `ARM Cortex-M4` `Linker Scripts` `OpenOCD` `STM32F4`

<br/>

**[Linux Wireless Kernel Patch](https://github.com/zaidahmad16/mac80211-ht-downgrade-fix)** &nbsp;·&nbsp; `[ OK ]` 54 Mbps → 1 Gbps

My Wi-Fi was capped at 54 Mbps. Should have been 1 Gbps. I traced the bug through the mac80211 stack, wrote the patch, and fixed it in the kernel.

`C` `Linux Kernel` `Wireless Networking` `mac80211`

<br/>

**[Nintendo DS Business Card](https://github.com/zaidahmad16/DS_Business_Card)** &nbsp;·&nbsp; `[ OK ]` runs on real hardware

My business card boots on a Nintendo DS. Plug it in, play a short game, get my contact info at the end. Pure C, no SDK game engine.

`C` `NDS SDK` `ARM` `Homebrew`

<br/>

**[Ghost Hunting Simulation](https://github.com/zaidahmad16/COMP2401-Final-Project)** &nbsp;·&nbsp; `[ OK ]` 0 deadlocks / 1,000+ ticks

A ghost hunting simulation in C where every actor is its own POSIX thread on shared memory. Spent a while on the deadlock prevention.

`C` `POSIX Threads` `Semaphores` `Linux`

---

### `systemctl status experience`

**● business-analyst.service** — Immigration, Refugees and Citizenship Canada (FSWEP) &nbsp;·&nbsp; *Jun – Aug 2026*
&nbsp;&nbsp;Turned vague, unquantified business-owner claims into auditable requirements — wrote the high-level business requirements for a governed low-code platform, and reworked the department's recurring annual change-request process so most updates became fast edits to precedent instead of full redrafts.

**● dev-volunteer.service** — Carleton Computer Science Society &nbsp;·&nbsp; *May – Aug 2026*
&nbsp;&nbsp;Added type-ahead search, a core-course filter, and a force-directed d3 visual entry point to the CS Society's course-graph explorer — mostly React/TypeScript, built on top of an existing dagre layout engine without breaking it.

**● logistics-coordinator.service** — cuHacking &nbsp;·&nbsp; *Sep 2025 – active*
&nbsp;&nbsp;Helping run Carleton's annual hackathon. Venues, schedules, sponsors — the stuff that has to work for everything else to work.

---

### `lsmod` — loaded skill modules

**Languages**

<img src="https://skillicons.dev/icons?i=c,cpp,java,python,js,ts,go&theme=dark" />

**Web & Backend**

<img src="https://skillicons.dev/icons?i=react,nextjs,nodejs,express,fastapi,tailwind,postgresql,mongodb,firebase,supabase&theme=dark" />

**Infra & Tooling**

<img src="https://skillicons.dev/icons?i=linux,git,githubactions,docker,aws,vercel,grafana,prometheus,bash&theme=dark" />

**Embedded & Systems**

`STM32` `ARM Cortex-M4` `POSIX Threads` `DKMS` `devkitARM` `Raw Sockets`

---

### `/boot/config` — education

**B.Sc. Computer Science** &nbsp;·&nbsp; AI & Machine Learning stream, Minor in Mathematics &nbsp;·&nbsp; Carleton University &nbsp;·&nbsp; *2024 – 2029*

`Data Structures & Algorithms` `C/C++` `Linear Algebra` `Discrete Structures II` `Web Applications`

Government of Canada Reliability Status Security Clearance &nbsp;·&nbsp; *Issued 2026*

---

<br/>

<div align="center">

![GitHub Stats](https://github-readme-stats.vercel.app/api?username=zaidahmad16&show_icons=true&theme=github_dark&hide_border=true&title_color=ffffff&text_color=888888&icon_color=4493f8&bg_color=0d1117)&nbsp;
![Top Languages](https://github-readme-stats.vercel.app/api/top-langs/?username=zaidahmad16&layout=compact&theme=github_dark&hide_border=true&title_color=ffffff&text_color=888888&bg_color=0d1117)

<sub>uptime: since 2024 · load average: manageable · `git commit -m "still building"`</sub>

</div>
