<div align="center">

```mermaid
flowchart TB
    A[Reverse Engineering] --> B[1. Define Objective and Scope]
    B --> B1[Target platform and file type]
    B --> B2[Authorization, isolation, and safety]
    B --> B3[Expected learning outcomes]

    B --> C[2. Initial Triage]
    C --> C1[Identify format, architecture, and compiler clues]
    C --> C2[Calculate hashes and inspect metadata]
    C --> C3[Extract strings, imports, exports, and sections]

    C --> D{3. Select Analysis Path}

    D -->|Static| E[Static Analysis]
    E --> E1[Disassembly]
    E --> E2[Decompilation]
    E --> E3[Control-flow and call-graph recovery]
    E --> E4[Data-flow and structure recovery]

    D -->|Dynamic| F[Dynamic Analysis]
    F --> F1[Execute in an isolated laboratory]
    F --> F2[Debug and trace instructions]
    F --> F3[Monitor processes, files, registry, and APIs]
    F --> F4[Observe network and memory behavior]

    E --> G[4. Program Understanding]
    F --> G
    G --> G1[Locate entry points and key routines]
    G --> G2[Rename functions and variables]
    G --> G3[Recover algorithms and data structures]
    G --> G4[Document findings and evidence]

    G --> H[5. Validation and Reporting]
    H --> H1[Cross-check static and dynamic evidence]
    H --> H2[Reproduce important observations]
    H --> H3[Write technical report and mitigations]
    H --> H4[Ethics, legal limits, and responsible disclosure]

    subgraph T[Reverse-Engineering Toolset]
      direction LR
      T1["Binary Triage<br/>file, strings, hashes, Detect It Easy"]
      T2["Disassemblers and Decompilers<br/>Ghidra, IDA Free, Cutter, JADX"]
      T3["Debuggers<br/>GDB, LLDB, WinDbg, x64dbg"]
      T4["Dynamic Monitoring<br/>Process Monitor, Process Explorer, strace, ltrace"]
      T5["Memory and Network<br/>Volatility, Wireshark, tcpdump"]
      T6["Mobile and Managed Code<br/>Apktool, JADX, dnSpyEx, ILSpy"]
      T7["Automation<br/>Python, Ghidra scripts, YARA"]
      T8["Documentation<br/>Markdown, diagrams, evidence log"]
    end

    E -. uses .-> T2
    F -. uses .-> T3
    F -. uses .-> T4
    F -. uses .-> T5
    C -. uses .-> T1
    G -. uses .-> T6
    G -. uses .-> T7
    H -. uses .-> T8

    classDef phase fill:#0f4c81,color:#fff,stroke:#083354,stroke-width:2px;
    classDef activity fill:#eaf3fb,color:#102a43,stroke:#5b8db8;
    classDef decision fill:#fff4cc,color:#5c4400,stroke:#c79800,stroke-width:2px;
    classDef tool fill:#edf8ef,color:#173d20,stroke:#58a66a;
    classDef governance fill:#fbecef,color:#5b1722,stroke:#c65b6d;

    class A,B,C,E,F,G,H phase;
    class D decision;
    class B1,B2,B3,C1,C2,C3,E1,E2,E3,E4,F1,F2,F3,F4,G1,G2,G3,G4,H1,H2,H3 activity;
    class H4 governance;
    class T1,T2,T3,T4,T5,T6,T7,T8 tool;
```

# **`Awesome`** Reverse Engineering Resources [![Awesome](https://awesome.re/badge.svg)](https://awesome.re)
</div>

[![YouTube](https://img.shields.io/badge/YouTube-%23FF0000.svg?style=for-the-badge&logo=YouTube&logoColor=white)]() 
[![Reddit](https://img.shields.io/badge/Reddit-FF4500?style=for-the-badge&logo=reddit&logoColor=white)]()

<p align="center">
    <a href="https://github.com/cybersecurity-dev/"><img height="25" src="https://github.com/cybersecurity-dev/cybersecurity-dev/blob/main/assets/github.svg" alt="GitHub"></a>
    &nbsp;
    <a href="https://www.youtube.com/@CyberThreatDefense"><img height="25" src="https://github.com/cybersecurity-dev/cybersecurity-dev/blob/main/assets/youtube.svg" alt="YouTube"></a>
    &nbsp;
    <a href="https://cyberthreatdefence.com/my_awesome_lists"><img height="20" src="https://github.com/cybersecurity-dev/cybersecurity-dev/blob/main/assets/blog.svg" alt="My Awesome Lists"></a>
    <img src="https://github.com/cybersecurity-dev/cybersecurity-dev/blob/main/assets/bar.gif">
</p>

## 📖 Contents
- [Books](#books)
- [Videos](#videos)
- [My Other Awesome Lists](#my-other-awesome-lists)
- [Contributing](#contributing)
- [Contributors](#contributors)

### Learning Hub
* [FLARE Learning Hub](https://github.com/mandiant/flare-learning-hub)

### Books
* Intel
    * [Practical Reverse Engineering: x86, x64, ARM, Windows Kernel, Reversing Tools, and Obfuscation](https://www.amazon.com/Practical-Reverse-Engineering-Reversing-Obfuscation/dp/1118787315)
    * [Reversing: Secrets of Reverse Engineering](https://www.amazon.com/Reversing-Secrets-Engineering-Eldad-Eilam/dp/0764574817)
    * [x86 Software Reverse-Engineering, Cracking, and Counter-Measures](https://www.amazon.com/x86-Software-Reverse-Engineering-Cracking-Counter-Measures/dp/1394199880)
* ARM
    * [Blue Fox: Arm Assembly Internals and Reverse Engineering](https://www.amazon.com/Blue-Fox-Assembly-Internals-Analysis/dp/1119745306)

### Videos
* [RE//verse 2025: How to Find Fully-Remote Bugs with Reverse Engineering (Natalie Silvanovich)](https://youtu.be/UOr1F-Tx1Zg?si=wArIBp0JG87jfNZr)

#### Video Series
* [Introduction to Reverse Engineering by @olivestemlearning](https://youtube.com/playlist?list=PL2EF13wm-hWClpBrC4eCLD4NcdXiLsLEb&si=82sd9_0nFiSMJWms)

### CTF
* [The Flare-On Challenge](https://flare-on.com/)

### AI Reverse Engineering Agent
- [ReAgent](https://github.com/Dryxio/reagent)

##

### My Other Awesome Lists
You can access the my other awesome lists [here](https://cyberthreatdefence.com/my_awesome_lists)

### Contributing
[Contributions of any kind welcome, just follow the guidelines](contributing.md)!

### Contributors
[Thanks goes to these contributors](https://github.com/cybersecurity-dev/awesome-reverse-engineering-resources/graphs/contributors)!

### License
[![CC0](http://mirrors.creativecommons.org/presskit/buttons/88x31/svg/cc-zero.svg)](http://creativecommons.org/publicdomain/zero/1.0)

[🔼 Back to top](#awesome-reverse-engineering-resources-)
