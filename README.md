#🔍 Cipher: Binus Cyber AI Festival - Interactive Log Analysis Simulation at Digital Forensic Analysis Booth 

[![Live Demo](https://img.shields.io/badge/Live-Demo%20on%20GitHub%20Pages-blue?style=for-the-badge)]([https://heiriko.github.io/Cipher-Digital-Forensic-Analysis-Log/](https://heiriko.github.io/Cipher-DFA-Log/))
[![Docker](https://img.shields.io/badge/Docker-Containerized-2496ED?style=for-the-badge&logo=docker&logoColor=white)](Dockerfile)

An interactive, browser-based Digital Forensics and Incident Response (DFIR) simulation challenge designed to guide users through identifying real-world attack chains via security telemetry logs.

🏆 **Recognition:** Awarded **"Most Voted Booth"** at the **Cipher Cyber AI Festival 2026** (Mall of Alam Sutera).

## 📖 Scenario Overview
An enterprise incident occurs at Cipher Corp. Participants step into the role of a Forensic Analyst to analize company logs and reconstruct the intrusion kill chain:
1. **Initial Access:** Spotting deceptive spear-phishing domain indicators (`@cipher-secure.com`).
2. **Account Compromise:** Identifying anomalous concurrent authentication across geographical anomalies (Jakarta vs. Minsk, Belarus).
3. **Malware Execution:** Detecting defense-evasion masquerading executables (`svch0st.exe`).
4. **Lateral Movement:** Tracking privilege escalation into IT administrator accounts.
5. **Impact & Exfiltration:** Documenting unauthorized database exports and log anti-forensics / tampering.

---
## How to Run

### Option 1: Live Web Demo (Instant)
Access the running application directly via [GitHub Pages Demo](https://heiriko.github.io/Cipher-DFA-Log/).

### Option 2: Docker Container (Local Deployment)
Ensure Docker is installed and running, then execute:

```bash
docker build -t cipher-dfir-lab .
docker run -d -p 8080:80 --name cipher-app cipher-dfir-lab
