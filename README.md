# 🛡️ Civic Asset Recovery Network (CARN) — Premium P2P Edition

Welcome to **CARN**, the next-generation premium iteration of the Civic Asset Recovery Network. This version introduces **Strict Peer-to-Peer Privacy Firewalls**, a fully **Decentralized Proof-of-Authority (PoA) Ledger**, and a **Local Ollama LLM Cognitive Auditing Engine** powered exclusively by the `llama3.2:1b` model.

---

## ⚡ Key Highlights & Features

### 1. 🗳️ Proof-of-Authority Consensus Ledger
* **Consensus telemetry panel**: Highlighting live *Quorum Health (99.98%)*, *Quorum Height*, *Node Count*, and *Validator Trust Rank (99.9% Reputation)*.
* **Animated cryptographic ledger timeline**: Renders newly mined consensus blocks sliding onto the blockchain with unique SHA-256 hashes, timestamps, and copy actions.
* **Validator Quorum Modal**: Interactive review interface showcasing side-by-side claim details, TensorFlow similarity ratings, and claimant answers.
* **Mined Block Pipeline**: An animated 4-stage Proof-of-Authority mining simulation (Hashing ➔ Broadcasting ➔ Signing ➔ Committing).

### 2. 🔐 Absolute Peer-to-Peer Privacy Firewalls
* **Verification questionnaire lock**: The secure questionnaire modal and answers can *only* be opened and submitted by the exact owner who lost the item.
* **Route display lockout**: Active maps, routes, and meeting instructions are strictly blocked and cleared from memory if an unauthorized user attempts to view them or run console scripts.
* **Contact disclosure lock**: Municipal contact names and phone numbers remain masked and secure until *both* parties have signed off on the PoA ledger.
* **Personal records isolation**: Filtered select tables in both the **Verify** dashboard and the **AI Fusion** control panel ensure that users can only view claims directly involving their phone numbers.

### 3. 🧠 Local Ollama AI Fusion Engine (`llama3.2:1b` Locked)
* **Dedicated Ollama Settings card**: Connects directly to local Ollama installations over CORS (`http://localhost:11434`).
* **UI Badge Locking**: Model selection dropdown removed in favor of a sleek, hardcoded indicator: `🤖 Model: llama3.2:1b`.
* **Live Terminal-style Thoughts Logger**: Prints progress steps as the model reads, compares, and audits semantics, locations, and visuals.
* **Sanitized JSON Parser with Regex Recovery**: High resiliency parsing that handles markdown code blocks, comments, and trailing commas. If the model's text is corrupted, a fallback regex parser recovers key fields.
* **"Adopt LLM Weights" Toggle**: Instantly applies LLM-recommended signal weights (Visual, NLP, Proximity, Decay, Metadata) directly to active sliders.

---

## 🛠️ Quick Start Guide

### 1. Open the Web App
Because CARN is built as a highly responsive, glassmorphic client-side application, you can run it in two ways:

#### Option A: Direct Local Host (Recommended)
This runs a lightweight local server, which allows the browser to easily handle GPS coordinates and Ollama CORS calls:
1. Open PowerShell or Command Prompt.
2. Start the local server:
   ```bash
   node "C:\Users\mbm54\.gemini\antigravity\brain\96ccc58f-5432-4728-b549-b7bf6545be08\scratch\server.js"
   ```
3. Open your browser and navigate to: **[http://localhost:5000/](http://localhost:5000/)**

#### Option B: Direct File Launch
Double-click [new_app.html](file:///c:/Hackathon/carn%202/new_app.html) or open it using the `/browser` slash command.

---

### 2. Set Up Ollama Local LLM
To use the AI Fusion tab, ensure your local Ollama server is running and configured with CORS headers enabled:

1. **Pull the Llama 3.2 1B Model**:
   ```bash
   ollama pull llama3.2:1b
   ```
2. **Start the Ollama Server with CORS enabled** (Required for browser fetch calls):
   * **Windows (PowerShell)**:
     ```powershell
     $env:OLLAMA_ORIGINS="*" ; ollama serve
     ```
   * **macOS/Linux**:
     ```bash
     OLLAMA_ORIGINS="*" ollama serve
     ```
3. Open the **AI Fusion** tab, ensure the host is set to `http://localhost:11434`, and click **🔄 Connect**. Once online, the status badge will glow **🟢 Online**.

---

## 🧪 Step-by-Step Test Walkthroughs

The application comes pre-loaded with simulated sandbox database scenarios in `localStorage`. Log in with the following phone numbers to test specific flows:

### Scenario A: End-to-End P2P Claim (Golden Retriever dog `MP-992`)
* **Meera Krishnan (Owner)**: `+91 76543 21098`
* **Suresh Raina (Finder)**: `+91 65432 10987`

1. Log in as **Meera** (`+91 76543 21098`). Go to the **Verify** tab, select the **Golden Retriever** match, click **📝 Answer Questionnaire**, fill in details, and submit. Status transitions to `Awaiting Finder's Signature`.
2. Log out and log in as an attacker (**Vikram Seth** - `+91 99999 88888`). Verify that the match does not appear in your queue and that maps/contacts remain locked.
3. Log out and log in as **Suresh** (`+91 65432 10987`). Go to the **Verify** tab, click **🗳️ Review & Sign**, review Meera's answers side-by-side, and click **Approve & Mint Block** to run the mining simulation.
4. Setup coordinate offsets (or click **📍 Use GPS**) and click **Generate Secure Route** to unlock the interactive Leaflet meetup route!

---

### Scenario B: Multi-Sig Verification Handshake (Silver Rolex Watch `MP-994`)
* **Vikram Seth (Owner)**: `+91 99999 88888`
* **Karthik Raja (Finder)**: `+91 88888 77777`

1. Log in as **Vikram** (`+91 99999 88888`). Navigate to **Verify**, click **🗳️ Review & Sign** on the Rolex watch validation, and click **Approve & Mint Block**. The status registers as `Awaiting Finder's Signature` and locks the button.
2. Log out and log in as **Karthik** (`+91 88888 77777`). Navigate to **Verify**, click **🗳️ Review & Sign** on the Rolex watch, and click **Approve & Mint Block**.
3. Watch the blockchain mining simulation execute, after which the safe meetup location coordinates will immediately prompt to unlock the routing map!

---

## 📁 Repository Structure
```text
c:\Hackathon\carn 2\
├── new_app.html    # Standalone Premium Glassmorphic Web App
└── README.md       # Full project handbook (This file)
```

Developed as part of the **Civic Asset Recovery Network ** project. Security, privacy, and local cognitive intelligence, unified.
