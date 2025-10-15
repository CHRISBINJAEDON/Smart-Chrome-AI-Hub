# Smart-Chrome-AI-Hub
Smart Chrome AI Hub empowers students to build AI-powered apps and Chrome Extensions that work offline, protect privacy, and reduce environmental impact. Using Gemini Nano and client-side AI, it enables ethical, inclusive innovation—aligning with UN SDGs for education, equality, and sustainability.

# 🌐 Smart Chrome AI Hub

**Empowering Students, Privacy, and Sustainability with Client-Side AI**

Built by: Chrisbin Liana, Chrisbin Jaedon, Johan Danieo R  
Affiliation: Sacred Heart International School, Tamil Nadu, India  
Grades: 11th, 8th, 7th Standard

---

## 🚀 Overview

Smart Chrome AI Hub is a student-led platform that enables youth to build AI-powered web applications and Chrome Extensions—without servers, without internet, and without compromising privacy. Powered by Gemini Nano and Chrome’s built-in AI APIs, the Hub delivers a future-ready, client-side solution aligned with key UN Sustainable Development Goals (SDGs).

---

## 🌟 Features

- 🗣️ **Multimodal Input**: Supports text, image, and audio via Prompt API  
- 🔐 **Client-Side AI**: All processing happens locally for privacy and speed  
- 🌐 **Multilingual Support**: Translator API enables global collaboration  
- 📄 **Summarization & Rewriting**: Uses Summarizer and Rewriter APIs  
- ✏️ **Grammar & Writing Tools**: Proofreader and Writer APIs included  
- 📶 **Offline Access**: Works without internet for low-connectivity regions  
- 🌱 **Sustainable Design**: No server costs, low carbon footprint

---

## 🧰 Tech Stack

- **Frontend**: React.js  
- **AI Engine**: Gemini Nano (client-side)  
- **Realtime Logic**: Firebase AI Logic  
- **Chrome APIs Used**:
  - Prompt API
  - Translator API
  - Summarizer API
  - Rewriter API
  - Writer API
  - Proofreader API

---

## 🛠️ Setup Instructions

```bash
# Clone the repository
git clone [https://github.com/your-username/smart-chrome-ai-hub.git](https://github.com/CHRISBINJAEDON/Smart-Chrome-AI-Hub.git)
cd smart-chrome-ai-hub

# Install dependencies
npm install

# Start the development server
npm start.
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
