# Samurai

Samurai is a **high-performance, low-latency** Linux kernel optimized for workloads that demand extreme responsiveness. It is **not a generic-use kernel**—it is stripped down to the bare essentials, built for **Edge, VoIP, Gaming, and VPNs**, where every microsecond counts.

## ⚠️ Important Considerations

- **Specialized Kernel:** Not designed for general-purpose use. Samurai is highly optimized and minimal—don’t expect it to work on your smart fridge. 🧊
- **EXTREME SECURITY WARNING:** This kernel prioritizes maximum performance by disabling virtually all security mitigations. This includes, but is not limited to, Spectre/Meltdown/L1TF/SSB mitigations, SELinux, and other hardening measures. **This configuration is HIGHLY INSECURE and should ONLY be used in trusted, isolated environments where security is explicitly NOT a concern.** If security is a priority for your use case, you MUST re-enable the necessary security mechanisms.
- **Minimal Drivers:** Limited hardware support due to the removal of unused drivers. Verify compatibility before use.
- **No Extensive Debugging:** Focus on performance means minimal logging and debugging features. Troubleshooting may be more challenging.

## 🔥 Key Features

- **Extreme Low Latency:** Configured with **PREEMPT_RT** and a **Tickless Kernel (NO_HZ_FULL @ 250Hz)** optimized for ultra-responsive performance.
- **Lightweight & Minimal Footprint:** Unused modules, drivers, and file systems removed for a streamlined footprint and reduced overhead.
- **Performance-Focused:** Deliberately excludes **SELinux, comprehensive CPU security mitigations, and excessive logging** to maximize efficiency and minimize performance impact.
- **Optimized I/O Performance:** Uses **mq-deadline** scheduler for reduced disk latency.

---

## 🤝 Contributions
Samurai is built for speed, but there's always room for improvement. Have ideas? **Fork the repo, tweak it, and submit a PR.** We welcome optimizations and performance hacks!
