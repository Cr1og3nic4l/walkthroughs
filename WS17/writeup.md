# WS17 – Windows Server 2017 Privilege Escalation

## 🛠️ Tools Used
- CMD / MS-DOS
- Basic Windows enumeration
- TryHackMe platform
- ChatGPT for technical support

---

## 🧭 Steps

### 1. Initial Access
- Connected to the Windows Server 2017 machine provided by TryHackMe.
- Identified user account and basic directory structure using `dir`, `cd`, and `whoami`.

### 2. User Flag
- Navigated to: `C:\Users\bill\Desktop`
- Found the file: `user.txt`
- Used the command:
  ```cmd
  type user.txt
  ✅ User Flag: 8bd7992fbe8a6ad22a63361004cfcedb

3. Privilege Escalation
Gained SYSTEM-level access (method not disclosed here due to TryHackMe rules).

Searched through C:\Windows\System32 for possible flag locations.

Found a flag in a location typically used to store sensitive data like password hashes.

4. System Flag
Used type to read the second flag once the file was found.

🔍 Notes
I chose to follow my own path using MS-DOS/CMD knowledge instead of strictly following the THM tutorial.

My familiarity with MsDos gave me an edge in navigating and finding flags quickly.

🧠 Lessons Learned
Don’t underestimate basic CMD skills — they’re still powerful in CTFs.

Always check default user desktops and system directories for flags.

Even when you're stuck, breaking the path and experimenting leads to progress.

📚 Resources
TryHackMe official room: Blue
Windows Privilege Escalation Cheat Sheets
