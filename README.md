# ForgeOS
> *"The OS that builds with you"*

ForgeOS is an AI-integrated operating system layer designed to make vibe-coding a reality — where the AI doesn't just suggest code, it **manufactures entire projects autonomously**, directly interfacing with your hardware, filesystem, and development environment.

---

## Core USPs

### 1. Hardware-Aware AI Context
ForgeOS runs AI agents as **OS-level daemons**, not apps. The AI knows your CPU core availability, RAM headroom, and disk I/O in real time. It dynamically decides how many parallel agents to spin up based on live system state.

---

### 2. Persistent Project Memory at the Filesystem Level
Every project directory gets a hidden `.forge/` context folder. Inside, the AI stores:
- Why each file was created
- Inter-file dependency maps
- The last recorded developer intent
- Agent task history

**No other tool does this natively.** Competitors are stateless per-session. ForgeOS *remembers*.

---

### 3. Raspberry Pi as a Dedicated Inference Node
This is the **killer differentiator**.

| Device | Role |
|---|---|
| Your Laptop (i5-12450H) | IDE, UI, heavy compilation |
| Raspberry Pi | Runs a lightweight local model 24/7 (Phi-3 Mini / Gemma 2B via Ollama) |

Your Pi becomes a **personal always-on AI brain** on your local network. No cloud. No API costs. No rate limits. Low latency. You own the entire stack.

---

### 4. Wayland Compositor Hook
ForgeOS integrates with the **Wayland compositor layer** on KDE Plasma. When you open a file manager or switch windows, the AI pre-indexes your project in the background — before you've even asked it anything.

Screen-aware context, zero manual setup.

---

### 5. Autonomous Git Loop
The AI doesn't just write code. It:
1. Writes the file
2. Runs the tests
3. Commits with a generated commit message
4. Pushes if tests pass
5. **Only pings you when something breaks**

True non-interactive development sessions.

---


## Reference Hardware

This project was designed and tested on:

| Component | Spec |
|---|---|
| **Device** | Lenovo IdeaPad Slim 5 14IAH8 |
| **Processor** | 12× Intel Core i5-12450H |
| **RAM** | 16 GiB (15.3 GiB usable) |
| **GPU** | Intel Graphics (integrated) |
| **OS** | EndeavourOS |
| **Desktop** | KDE Plasma 6.5.5 (Wayland) |
| **Kernel** | 6.18.5-arch1-1 (64-bit) |
| **Inference Node** | Raspberry Pi (local LAN) |

---

## Vision

Most AI coding tools make you a **better prompter**.

ForgeOS makes you a **director**. You describe what you want built. The OS handles the rest — files, structure, commits, tests, iterations. You step in only when creative direction is needed.

This is not an IDE plugin. This is not a CLI wrapper.

**This is the OS as your co-engineer.**

---

## License

MIT License — open to the community, built for builders.

---

*Built with intent on EndeavourOS. Powered by local inference. Directed by humans.*
