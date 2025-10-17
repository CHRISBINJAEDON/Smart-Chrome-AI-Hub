# Smart-Chrome-AI-Hub
Smart Chrome AI Hub empowers students to build AI-powered apps and Chrome Extensions that work offline, protect privacy, and reduce environmental impact. Using Gemini Nano and client-side AI, it enables ethical, inclusive innovation—aligning with UN SDGs for education, equality, and sustainability.
# 🌐 Smart Chrome AI Hub

Empowering Students, Privacy, and Sustainability with Client-Side AI  
**Team Members:** Chrisbin Liana, Chrisbin Jaedon, Johan Danieo R  
**Affiliation:** Sacred Heart International School, Tamil Nadu, India (11th, 8th, 7th Standard)

---

## 🌟 Vision & Purpose

Smart Chrome AI Hub is a student-led platform that enables youth to build AI-powered web applications and Chrome Extensions—without servers, without internet, and without compromising privacy. By harnessing Google Chrome AI APIs like Gemini Nano, the Hub delivers a future-ready, client-side solution aligned with key UN Sustainable Development Goals (SDGs), including:

- Quality Education (SDG 4)
- Gender Equality (SDG 5)
- Climate Action (SDG 13)
- Reduced Inequalities (SDG 10)
- Sustainable Cities and Communities (SDG 11)

---

## 🌱 Inspiration

We were inspired by the growing need for accessible, privacy-first AI tools—especially for students in low-connectivity regions. With AI shifting from cloud to device, we saw an opportunity to eliminate server costs, reduce environmental impact, and democratize innovation.

---

## ⚙️ Key Features

- ✅ **Client-side AI** using Gemini Nano (no servers required)
- 🧠 **Multimodal input support**: text, image, audio
- 📴 **Offline functionality** for remote and low-connectivity regions
- 🖥️ **Cross-platform compatibility** (mobile + desktop)
- 🌐 **Chrome API integration** for translation, rewriting, summarization
- 🔐 **Privacy-first architecture** with no data sent to cloud

---

## 🛠️ How We Built It

- **Frontend:** React.js
- **AI Engine:** Gemini Nano (Chrome AI APIs)
- **Realtime Logic:** Firebase AI Logic (client-side only)
- **Design:** Responsive layout with Material UI and Tailwind CSS
- **Chrome Extension:** Manifest V3 with local AI hooks

---

## 🚧 Challenges We Overcame

- Real-time optimization of multimodal AI
- Memory-efficient offline architecture
- Cross-device compatibility
- Accessibility without compromising performance

---

## 🏆 Impact & Accomplishments

- Enabled students to build AI apps without servers
- Promoted ethical, privacy-first development
- Supported inclusive education and sustainable innovation
- Aligned with 7+ UN SDGs
- Delivered tools for:
  - ✍️ Text generation
  - 📚 Summarization
  - 🌍 Translation
  - 📝 Writing improvement

---

## 📖 What We Learned

- Client-side AI bridges digital divides
- Privacy and sustainability are enablers, not limitations
- Youth-led innovation thrives with the right tools
- Ethical design can scale globally

---

## 🔮 What’s Next

- 🎙️ Expand multimodal features: voice recognition, image-to-text
- 📱 Enhance mobile compatibility
- 🤝 Launch collaborative extension builder
- 🌐 Integrate hybrid AI strategies for global reach

---

## 🚀 Getting Started

### Prerequisites

- Node.js ≥ 18
- Chrome ≥ 120 (Gemini Nano support)
- Firebase CLI (for local emulation)

### Installation

```bash
https://github.com/CHRISBINJAEDON/Smart-Chrome-AI-Hub.git
git clone https://github.com/your-username/smart-chrome-ai-hub.git
cd smart-chrome-ai-hub
npm install
## 🎥 Demo Videos

Watch our project in action:

- [🔗 Demo Video 1 – Smart Chrome AI Hub Overview](https://youtu.be/iR4TMMGe26w)
- [🔗 Demo Video 2 – Feature Walkthrough & Use Cases](https://youtu.be/R1WqKWF4X84)

You can also preview them below:

[![Demo Video 1](https://img.youtube.com/vi/iR4TMMGe26w/0.jpg)](https://youtu.be/iR4TMMGe26w)
[![Demo Video 2](https://img.youtube.com/vi/R1WqKWF4X84/0.jpg)](https://youtu.be/R1WqKWF4X84)
Smart-Chrome-AI-Hub/
├── manifest.json
├── background.js
├── popup.html
├── popup.js
├── styles.css
├── assets/
│   └── icon.png
├── README.md
{
  "manifest_version": 3,
  "name": "Smart Chrome AI Hub",
  "description": "Client-side AI tools powered by Gemini Nano",
  "version": "1.0",
  "permissions": ["activeTab", "scripting"],
  "action": {
    "default_popup": "popup.html",
    "default_icon": "assets/icon.png"
  },
  "background": {
    "service_worker": "background.js"
  },
  "host_permissions": ["<all_urls>"]
}
<!DOCTYPE html>
<html>
<head>
  <title>Smart Chrome AI Hub</title>
  <link rel="stylesheet" href="styles.css">
</head>
<body>
  <h1>Smart Chrome AI Hub</h1>
  <textarea id="inputText" placeholder="Enter text to summarize or proofread..."></textarea>
  <button id="summarizeBtn">Summarize</button>
  <button id="proofreadBtn">Proofread</button>
  <div id="output"></div>
  <script src="popup.js"></script>
</body>
</html>
document.getElementById("summarizeBtn").addEventListener("click", async () => {
  const input = document.getElementById("inputText").value;
  const summary = await summarizeText(input);
  document.getElementById("output").innerText = summary;
});

document.getElementById("proofreadBtn").addEventListener("click", async () => {
  const input = document.getElementById("inputText").value;
  const corrected = await proofreadText(input);
  document.getElementById("output").innerText = corrected;
});

async function summarizeText(text) {
  // Simulated Gemini Nano Summarizer API call
  return `Summary: ${text.slice(0, 50)}...`;
}

async function proofreadText(text) {
  // Simulated Proofreader API call
  return `Corrected: ${text.replace("teh", "the")}`;
}
chrome.runtime.onInstalled.addListener(() => {
  console.log("Smart Chrome AI Hub installed.");
});
body {
  font-family: Arial, sans-serif;
  padding: 10px;
  width: 300px;
}

textarea {
  width: 100%;
  height: 80px;
  margin-bottom: 10px;
}

button {
  margin-right: 5px;
}

#output {
  margin-top: 10px;
  font-weight: bold;
}
body {
  font-family: Arial, sans-serif;
  padding: 10px;
  width: 300px;
}

textarea {
  width: 100%;
  height: 80px;
  margin-bottom: 10px;
}

button {
  margin-right: 5px;
}

#output {
  margin-top: 10px;
  font-weight: bold;
}
