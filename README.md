# 🛡️ FocusGuard

**Reclaim Your Attention, One Quote at a Time.**

> *"Distraction is the thief of dreams."*

**FocusGuard** isn't just a site blocker; it's a gentle nudge back to reality. Designed for students, developers, and anyone fighting the scroll-hole, this Chrome Extension silently tracks your time on distracting sites and intervenes with wisdom when you've had enough.

---

## ✨ Why FocusGuard?

We all do it. You open Twitter for "5 minutes" and suddenly it's an hour later. **FocusGuard** solves this by enforcing the limits you set.

* 🛑 **Strict & Friendly Blocking:** When your time is up, we don't just notify you—we redirect you to a calming "Time's Up" page with a motivational quote.
* 🌗 **Midnight Mode:** A stunning, deep-dark UI that respects your eyes.
* 🔒 **Privacy First:** Your browsing data never leaves your machine. No clouds, no tracking servers.
* ⚡ **Lightweight:** Runs efficiently in the background using Chrome's latest **Manifest V3** technology.

---

## 🚀 Features at a Glance

| Feature | Description |
| :--- | :--- |
| **⏱️ Smart Tracking** | Automatically counts seconds spent on specific domains (YouTube, Reddit, etc.). |
| **🚫 Strict Redirect** | Redirects the tab to a blocked page immediately when the limit is exceeded. |
| **🎛️ Total Control** | You set the daily limit (default: 30m). You choose the blocked sites. |
| **🔋 Battery Friendly** | Uses Chrome `Alarms` and `Service Workers` so it doesn't drain your laptop battery. |

---

## 🛠️ Installation Guide

Since this is a custom-built extension, you can install it directly in Developer Mode:

### Step 1: The Setup
Clone this repository or download the source code and locate the **`FOCUSGUARD`** folder containing:
* `manifest.json`
* `background.js`
* `popup.html` & `popup.css`
* `popup.js`
* `blocked.html` *(The page you see when time is up)*
* `icon.png`

### Step 2: Load in Chrome
1. Open Google Chrome and navigate to `chrome://extensions` in the address bar.
2. Toggle **Developer Mode** 🔛 (top-right corner switch).
3. Click the **Load unpacked** button (top-left).
4. Select the **`FOCUSGUARD`** folder inside this repository.
5. 🎉 **Success!** Pin the **FocusGuard** icon to your Chrome toolbar.

---

## 🎮 Usage

### 1. The Dashboard
Click the extension icon to open the popup:
* **Stats:** See exactly how many minutes you've spent on each site today.
* **Limit:** Change your daily allowance (e.g., 45 mins) and click **Save**.

### 2. Managing Distractions
By default, FocusGuard tracks the **"Big Five"**:
* `youtube.com`
* `twitter.com`
* `reddit.com`
* `facebook.com`
* `instagram.com`

* **To Add a Site:** Type the domain (e.g., `netflix.com`) in the input box and click `+`. The extension automatically cleans URL inputs to extract the domain.
* **To Remove a Site:** Click the `×` button next to the site name in the list.

---

## 📂 Under the Hood

Here is how the extension is structured:

```text
FOCUSGUARD/
├── 📄 manifest.json   # The Blueprint (Permissions & Manifest V3 Config)
├── 🧠 background.js   # The Brain (Time tracking logic & Alarms)
├── 🎨 popup.css       # The Look (Dark theme styling)
├── 🖥️ popup.html      # The Face (Structure of the extension popup)
├── ⚙️ popup.js        # The Muscle (Saves settings & updates UI via Chrome Storage)
└── 🚫 blocked.html    # The Enforcer (Redirect destination when time expires)

---

## 🔮 Roadmap

- [x] **Strict Mode:** Force redirect tabs when time is up.
- [ ] **History Graphs:** Visualize your focus progress over a week.
- [ ] **Focus Sounds:** Play ambient white noise while working.

---

### 💻 Made with ❤️ by **Team NOVUS** (Aditya Singh & Mayank Gupta)
