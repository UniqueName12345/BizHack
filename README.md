# BizHack

> **a fork of BizHawk with no rules, only RAM**

Welcome to BizHack: the unholy spawn of tool-assisted speedruns and raw memory corruption.  
Think BizHawk, but with direct RAM write access mid-run. Why wait for the game to let you win, when you can *rewrite the game itself*?

This project **will never** be supported by TASVideos. This is for glitchers, hackers, memory editors, and deranged god-TASers only. You know who you are.

---

![hacker aesthetic](/media/hacker_vibes.png)  
*A TAS so powerful, even the emulator fears it.*

---

## 💀 What is BizHack?

BizHack is a multi-system emulator written in C# and C++ like its parent, BizHawk, but with a key difference:  
**TAS movies can now execute frame-precise RAM edits.**  
That means during playback, your TAS can do things like:
- Patch your health to 999 every frame
- Replace your character's sprite with the final boss
- Rewrite RNG seeds into all 7s
- Make the game crash *on purpose*
- Inject save data, force flags, bypass sanity checks
- Enter level 3 by flipping one byte in RAM instead of walking

There are no restrictions. The TAS **is the code**.

---

## 💾 Features

- All the standard BizHawk tools you love: savestates, Lua scripting, TAStudio, input recording.
- But also:  
  🔧 **Memory injection scripting** per frame  
  🔧 Custom `MemoryAction` format inside `.tasproj` files  
  🔧 TAStudio panel for RAM poking  
  🔧 Real-time memory edits that play back deterministically

---

## ⚠️ WARNING

This fork is for *fun*, not for TASVideos compatibility.

- Don’t expect desync-safe submissions.  
- Don’t expect praise.  
- Do expect glitchy chaos, corrupted saves, and games screaming in binary.

You are no longer *playing* the game. You are **rewriting its destiny**.

---

## 💻 Installing

Same as BizHawk:

1. Download the latest build from [Releases](https://github.com/yourname/BizHack/releases)
2. Unzip and run `EmuHawk.exe`
3. Add `.tasproj` files with RAM instructions, or open TAStudio and start poking bytes mid-run
4. Laugh maniacally

---

## 📂 New TAS Format Additions

Inside your `.tasproj`, you’ll now see:
```json
"MemoryActions": [
  { "Frame": 123, "DomainName": "Main RAM", "Address": 65536, "Value": 255 },
  { "Frame": 124, "DomainName": "WRAM", "Address": 0xDEAD, "Value": 0xBEEF }
]
````

These actions are deterministic and applied every time the frame plays, just like inputs.

---

## 🎥 TAS Like a Hacker

1. Load a game
2. Open TAStudio
3. Input buttons as normal
4. Add RAM edits on the same frames
5. Watch the game *obey*

Use this to:

* Force doors open
* Skip cutscenes entirely
* Activate glitches without setup
* Laugh in hexadecimal

---

## 🤝 Contributing

If you have ideas like “what if TAS scripts could also write to CPU registers?” or “can we swap ROM banks mid-frame?” — you belong here. Fork, break things, PR later.

---

## 🧨 License

MIT. Do what you want. But if Nintendo shows up at your house, we’ve never met you.

---

## 📛 Not Affiliated With:

* TASVideos.org
* Legitimate speedrunning
* Reality as you know it

---

## 👾 FAQ

**Q: Is this cheating?**
**A:** Yes. That’s the point.

**Q: Why isn't this allowed on TASVideos?**
**A:** Because it turns a TAS into a programmable game mod. Duh.

**Q: Can I use this to break games in new, terrible ways?**
**A:** Yes. Send screenshots.

---

## 💬 Support

You're on your own.
But if you're cool enough, you'll figure it out.

---

> *"Games are just memory maps waiting to be rewritten." – UniqueName12345*
