# BizHack

**A fork of BizHawk that cheats harder than reality.**

BizHack is an experimental fork of [BizHawk](https://github.com/TASEmulators/BizHawk), written in C#, designed exclusively for Windows, and **absolutely not TASVideos-approved**.

Unlike traditional TAS tools which simulate button inputs, BizHack lets you *become the machine*. Modify RAM, rewrite flags, kill collision, spawn impossible items, break frame rules — all without touching the controller. Why be good at the game when you can rewrite its soul?

⚠️ This tool is for entertainment, glitch research, chaos engineering, or possibly violating the Geneva Convention of TASing. **Use responsibly.**

---

## 🧠 Features (compared to base BizHawk)

- Everything BizHawk does: savestates, frame advance, full input control, Lua scripting, savestate rewinds...
- **Plus one forbidden feature:**
  > 🚨 Inject custom RAM writes per frame, per domain, with no restrictions.

That’s right. Want to zero out health every 3 frames? Set your X position to 9999? Make enemies fall through the floor? You can.

**You’re not playing the game anymore. You’re puppeteering the RAM.**

---

## 💻 Supported Platforms

- **Windows 10/11 only**
- 64-bit. No Linux. No Mono. No Apple. No compromise.

Why? Because I use Windows, and this isn't meant to be portable. If you're a Linux nerd, feel free to fork *this fork*.

---

## 🚀 Getting Started

1. Download from [Releases](https://github.com/YOURUSERNAME/BizHack/releases)
2. Extract into a fresh folder. Do **not** mix with regular BizHawk.
3. Run `EmuHawk.exe`
4. Load a game
5. Open the new **Memory Actions** panel in TAStudio
6. Inject chaos

---

## ✍️ RAM Manipulation API

Each memory action is:
```json
{
  "Frame": 1337,
  "DomainName": "System Bus",
  "Address": 0xDEAD,
  "Value": 0xBE
}
````

Memory actions can be:

* Replayed automatically during TAS playback
* Edited live in TAStudio
* Loaded from external JSON
* Triggered by Lua (with great danger)

---

## 🧪 Experimental

This project is:

* Not tested for determinism
* Not stable
* Not supported by TASVideos or any sane person

If a game softlocks, explodes, or summons the ghost of Shigeru Miyamoto — that’s on you.

---

## 🔥 Why?

Because scripting input is fun…
…but scripting **reality** is better.

BizHack is a tribute to the absurd potential of emulator tooling. It’s not about high score, it’s about high entropy.

---

## ⚠️ Legal, Ethical, and Other Disclaimers

* Do not submit TASes made in BizHack to TASVideos. They will be rejected faster than a frame-perfect lag skip.
* Do not use this to cheat in netplay. That’s just lame.
* All standard BizHawk licenses still apply.
* Don’t distribute copyrighted ROMs.
* Don’t assume this tool is safe for your data. Or your sanity.

---

## 🧠 Support?

None. This is a solo passion project. If it breaks, read the source code.
Forks welcome. Feature requests will be ignored unless they're funny.

---

## 🎤 Final Words

> "Tool-Assisted Speedruns are about precision.
> BizHack is about **power**."

Happy corrupting.
— Smurf Someone
