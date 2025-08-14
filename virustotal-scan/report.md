
# VirusTotal Analysis Report

## 📁 File Info
- **Filename:** infected.zip (contains `LBpjy.exe`)
- **File Size:** 763.40 KB (ZIP), 902.00 KB (EXE)
- **Compression:** AES Encrypted ZIP Archive
- **Hashes:**
  - **MD5:**
    - ZIP: `548c0a4d5bfe4628a64ae4c77aaac67b`
    - EXE: `f1fd4cf59c5cfb5e4ab5fd8570889f6b`
  - **SHA1:**
    - ZIP: `7a39d22d41cd40bd2cbdc80444af713e96eec56`
    - EXE: `48543fec63c09015380892c3dcfc411979c4b45`
  - **SHA256:**
    - ZIP: `f630d61a35d98b69b7d9e2220030dcf4752932860872142dfac8acda031bdc7`
    - EXE: `ae2a513b61febc225d5e374ab22dba754a3d38e49b7bbd442fe3f9bab16b8fb1`

---

## 🧪 Detection
| Engine | Detection |
|--------|-----------|
| 55/72 engines | Malicious (for `LBpjy.exe`) |
| Examples | Trojan, Stealer, Keylogger variants |
| Encrypted ZIP | 0/65 flagged (content not scanned) |

---

## 📡 Network Indicators

**Contacted Domains:**
- `api.telegram.org` – 3/94 detections
- `checkip.dyndns.org` – 0/94 detections
- `mail.gazitoomasyon.com.tr` – 0/94 detections
- `reallyfreegeoip.org` – 1/94 detections

**Contacted URLs:**
- `https://reallyfreegeoip.org/xml/1.254.1.255`
- Telegram bot API message-sending endpoints (multiple)
- IP: `107.167.163.178`

---

## 📊 Behavioral Summary
- **Suspicious DNS Queries:** IP lookup services (`api.ipify.org`) from non-browser processes.
- **Telegram Bot Communication:** Suspicious DNS queries to `api.telegram.org`.
- **Payload:** Drops and executes a Win32 EXE (`LBpjy.exe`).
- **Capabilities:**
  - Keylogging
  - Information stealing (passwords, system info)
  - Clipboard monitoring
  - Persistence via registry
  - WMI calls, anti-debugging
  - Communication with remote C2 via Telegram

---

## 🗣️ Community Insight
- **Votes:** Mostly negative (-12 community score for EXE)
- **ANY.RUN Sandbox Analysis:** Malicious activity detected; tags: evasion, snake, keylogger, telegram, stealer, smtp
- **Comments:** Indicate clear malicious intent and active exfiltration

---

## 🔐 Public Link
- [VirusTotal Public Scan Link – infected.zip](https://www.virustotal.com/gui/file/f630d61a35d98b69b7d9e2220030dcf4752932860872142dfac8acda031bdc7)
- [VirusTotal Public Scan Link – LBpjy.exe](https://www.virustotal.com/gui/file/ae2a513b61febc225d5e374ab22dba754a3d38e49b7bbd442fe3f9bab16b8fb1)
