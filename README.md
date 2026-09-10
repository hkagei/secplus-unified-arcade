# 🕹️ SY0-701 Unified Practice Arcade

> **Turn CompTIA Security+ study into an arcade game.**

**SY0-701 Unified Practice Arcade** is a browser-based study game designed to make preparing for the **CompTIA Security+ SY0-701** exam more engaging through timed drills, memory games, game-show-style questions, and interactive PBQ-style exercises.

Instead of studying one topic at a time through conventional flashcards, the arcade combines Security+ concepts into multiple game modes so you can practice **recognition, recall, sequencing, categorization, and scenario-based decision-making**.

**No framework. No build process. No dependencies. Just open the HTML file and play.**

---

## 🎮 Game Modes

The arcade currently includes **six different ways to study**.

### 1. ⚡ Multiple Choice — Speed Drill

Test your ability to quickly recognize Security+ concepts and definitions.

* Timed questions
* Multiple-choice answers
* Limited lives
* Score tracking
* Timer becomes more challenging as your score increases
* Immediate feedback
* Domain filtering

Perfect for rapid-fire acronym and terminology review.

---

### 2. 🧠 Matching Game — Recall

Match Security+ concepts with their definitions.

* Up to 8 pairs per round
* Concepts and definitions are shuffled
* Move counter
* Immediate visual feedback
* Domain filtering

This mode emphasizes **active recall rather than passive recognition**.

---

### 3. 🎡 Wheel of Fortune — Letters

A Security+-themed spin-the-wheel game.

Given a concept, use the wheel and letter guessing to uncover its definition.

* Spin for point values
* Guess individual letters
* Solve the complete definition
* Limited strikes
* Bank winnings
* Difficulty-based strike limits

It's essentially **Wheel of Fortune meets Security+ terminology**.

---

### 4. 💰 Jeopardy — Board Mode

Test yourself with a full Security+ Jeopardy-style board.

There are two separate boards:

#### Main Domains Board

* General Security Concepts
* Threats & Vulnerabilities
* Security Architecture
* Security Operations
* Program Management & Oversight

#### PBQ Subdomains Board

* AI & Zero Trust
* Crypto & Hardening
* Continuity & Response
* Detection & Logs
* Network & Access

Each board contains **five categories and five point levels ($100–$500)**.

---

### 5. 🔀 Sequence Lab — Order the Steps

Put cybersecurity processes in the correct order.

Current scenarios include topics such as:

* Incident Response phases
* BCDR recovery
* PKI certificate-chain construction
* Linux breach response
* Attack/kill-chain sequencing

Each scenario scores how many steps you placed in their correct positions and shows the correct position when you miss one.

This mode is particularly useful for memorizing **processes and operational workflows**, rather than individual definitions.

---

### 6. 🗺️ Placement Lab — Place the Controls

A PBQ-style categorization exercise.

Select an item and place it into the zone where it belongs.

Examples include:

* Zero Trust architecture
* Network security diagrams
* Security controls
* Hosts
* Traffic
* Detection/monitoring components

The game tracks:

* Correct placements
* Mistakes
* Scenario completion

This mode is intended to provide practice closer to the **conceptual reasoning required by performance-based questions (PBQs)**.

---

## 📚 Study Content

The arcade separates its study material into two major groups.

### Security+ Main Exam Domains

The application organizes its acronym bank across the five major SY0-701 areas:

1. **General Security Concepts**
2. **Threats, Vulnerabilities & Mitigations**
3. **Security Architecture**
4. **Security Operations**
5. **Security Program Management & Oversight**

### PBQ-Oriented Subdomains

The application separately maintains specialized practice areas for:

* Secure AI / RAG Configuration
* Zero Trust Architecture
* PKI & Cryptography
* Linux Breach Response
* BCDR & Recovery
* SIEM & SOAR
* Firewall ACL Rules
* Advanced Firewall Configuration
* IDS/IPS Alert Analysis
* Incident Response Phases
* Security Log Analysis
* Network Security Diagrams
* Subnetting & VLSM
* System Hardening
* Wireless AP Configuration

Keeping these two groups separate is intentional: the application is designed to distinguish **exam-domain terminology review** from **hands-on/PBQ-style scenario practice**.

---

## 🎯 Difficulty Levels

Multiple Choice and Wheel of Fortune support four difficulty levels:

| Difficulty   | Lives | Starting Time | Strikes |
| ------------ | ----: | ------------: | ------: |
| Easy         |     5 |        20 sec |       5 |
| Medium       |     3 |        15 sec |       3 |
| Hard         |     2 |        10 sec |       2 |
| Sudden Death |     1 |        12 sec |       1 |

**Sudden Death** is designed for high-pressure review: one mistake ends the run.

---

## 🎨 Customization

The arcade includes a built-in customization panel.

You can change:

* Dark / light mode
* Difficulty
* Accent color
* Correct-answer color
* Incorrect-answer color
* Warning color
* Preset color themes

The default interface uses a dark, terminal-inspired aesthetic with a grid background and monospace typography.

---

## 🚀 Getting Started

### Option 1 — Open Directly

Clone the repository:

```bash
git clone https://github.com/hkagei/secplus-unified-arcade.git
cd secplus-unified-arcade
```

Then open:

```text
index.html
```

in your web browser.

That's it.

There is currently **no package manager, build system, framework, or external dependency required**. The application is contained in a single HTML file with embedded CSS and JavaScript.

---

### Option 2 — Run a Local Web Server

For a more realistic browser environment, run a simple local server.

#### Python

```bash
python -m http.server 8000
```

Then visit:

```text
http://localhost:8000
```

#### Node.js

If you already have a static server available:

```bash
npx serve .
```

Then open the URL provided by the server.

---

## 🌐 GitHub Pages

Because the arcade is a static HTML/CSS/JavaScript application, it can also be hosted using **GitHub Pages**.

A typical deployment structure is simply:

```text
secplus-unified-arcade/
└── index.html
```

No compilation step is required.

---

## 🧩 Technology

The project intentionally keeps the technology stack lightweight:

* **HTML5**
* **CSS3**
* **Vanilla JavaScript**
* HTML `<canvas>` for the Wheel of Fortune
* Browser DOM APIs
* No external JavaScript frameworks
* No backend
* No database
* No build tools
* No npm dependencies

The entire application is currently implemented in `index.html`.

---

## 🗂️ Repository Structure

```text
secplus-unified-arcade/
│
├── index.html      # Complete arcade application
└── README.md       # Project documentation
```

The current repository intentionally keeps the project extremely portable: the application can be copied, downloaded, or hosted as a static site without additional setup.

---

## 🧠 Study Philosophy

The arcade is built around a simple idea:

> **Security+ preparation shouldn't have to feel like repeatedly flipping through flashcards.**

Different game modes target different learning skills:

| Game Mode        | Primary Skill        |
| ---------------- | -------------------- |
| Multiple Choice  | Recognition & speed  |
| Matching         | Active recall        |
| Wheel of Fortune | Terminology recall   |
| Jeopardy         | Broad-domain review  |
| Sequence Lab     | Process memorization |
| Placement Lab    | Scenario reasoning   |

The goal is to make it easier to repeatedly revisit concepts until they become **retrievable under pressure**, rather than simply familiar when seen on a flashcard.

---

## 🛡️ Security+ Disclaimer

This project is an **independent study aid** and is not affiliated with, endorsed by, or sponsored by CompTIA.

The application is intended to supplement—not replace—official CompTIA study materials, practice exams, course instruction, and other authoritative resources.

Security+ exam objectives and terminology may change over time. Always verify current exam requirements against the official CompTIA objectives.

---

## 🤝 Contributing

Suggestions, corrections, new questions, additional PBQ scenarios, and new game ideas are welcome.

Potential contributions include:

* New Security+ terminology
* Improved definitions
* Additional PBQ scenarios
* New sequence exercises
* New placement exercises
* Additional game modes
* Accessibility improvements
* Mobile UI improvements
* Performance improvements
* Bug fixes

When adding study content, prioritize:

1. Accuracy
2. Clear explanations
3. Alignment with SY0-701 concepts
4. Useful exam-oriented distinctions
5. Scenario-based reasoning where appropriate

---

## 💡 Future Ideas

Potential additions include:

* [ ] More PBQ-style simulations
* [ ] Full exam simulation mode
* [ ] Question difficulty tagging
* [ ] Missed-question review
* [ ] Persistent statistics
* [ ] Streak tracking
* [ ] High-score tracking
* [ ] Daily challenge
* [ ] Timed exam mode
* [ ] Custom question sets
* [ ] More networking/subnetting challenges
* [ ] More log-analysis scenarios
* [ ] Additional firewall/ACL exercises
* [ ] Drag-and-drop PBQs
* [ ] Keyboard shortcuts
* [ ] Accessibility improvements
* [ ] Mobile-first improvements
* [ ] Installable PWA support

---

## 📖 Current Content Focus

The arcade currently emphasizes concepts including:

* Security fundamentals
* Cryptography
* PKI
* Authentication & authorization
* Network security
* Wireless security
* Identity and access management
* Vulnerabilities and mitigations
* Incident response
* SIEM/SOAR
* IDS/IPS
* Firewalls and ACLs
* Zero Trust
* Secure AI/RAG concepts
* Linux hardening
* Business continuity and disaster recovery
* Security logging
* Network architecture
* Subnetting
* System hardening

The underlying content is embedded directly into the application rather than retrieved from an external API or database.

---

## ⭐ Why This Project?

**Security+ studying + arcade games = less boring studying.**

The project was created to turn repetitive Security+ review into something that feels more like a game than a traditional study session.

```text
STUDY
  ↓
PLAY
  ↓
MISS
  ↓
LEARN
  ↓
RETRY
  ↓
MASTER
```

---

## 📜 License

No separate license file is currently included in the repository.

If you intend for others to freely reuse, modify, or redistribute the project, consider adding an explicit open-source license such as MIT.
