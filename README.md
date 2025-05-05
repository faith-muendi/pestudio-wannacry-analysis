# 🔬 PEStudio Static Malware Analysis – wannacry.zip

This repository contains my initial static malware analysis of a suspicious file named `wannacry.zip`, performed using **PEStudio**. The goal is to assess potential threats using static inspection techniques without executing the file.

---

## 📌 Project Details

- **Analyst:** Faith Muendi  
- **Date:** May 5, 2025  
- **Tool Used:** [PEStudio v9.61](https://www.winitor.com/)  
- **File Name:** `wannacry.zip`  
- **SHA-256 Hash:**  
  `8739C76E681F900923B900C9DF0EF75CF421D39CAB854650C4B9AD1986A76D85`

---

## 🧪 Key Findings

- ✅ **Indicators flagged by PEStudio:** > 6  
- ✅ **VirusTotal Analysis:** 0/60 detections  
- 🧠 **AV Engines Used:** AVG, BitDefender, Kaspersky, Microsoft, Fortinet, etc.  
- ⚠️ **Suspicious file name:** Commonly associated with the WannaCry ransomware strain.

---

## 🖼️ Screenshot

![PEStudio Report Screenshot](./Screenshot.png)

> *This screenshot shows the VirusTotal section in PEStudio with 0 detections across 60 AV engines.*

---

## 🧠 Interpretation

Although VirusTotal shows a clean result (0 detections), the use of the name `wannacry.zip` and the presence of flagged indicators in PEStudio raise concern. This file may:
- Be packed or obfuscated
- Use evasion techniques to bypass static detection
- Require deeper **dynamic analysis in a sandboxed environment**

---

## 🛠️ Tools & Techniques Used

| Tool        | Purpose                         |
|-------------|----------------------------------|
| PEStudio    | Static file inspection & metadata |
| VirusTotal  | Cross-check with antivirus engines |
| Hashing (SHA-256) | File fingerprinting           |

---

## 🧭 Next Steps (Dynamic Analysis Plan)

- ✅ Extract inner contents of the ZIP (if any)
- ✅ Inspect PE headers, imports, exports
- ❗ Execute in a sandbox (like Any.Run or Cuckoo)
- ❗ Monitor file, process, network behavior

---

## 🏁 Conclusion

This analysis is part of my practical cybersecurity learning path, focusing on malware detection and reverse engineering techniques. PEStudio provides a strong foundation for recognizing early indicators of potentially malicious files before execution.

---

> 📚 *This project is one of several in my cybersecurity journey, including vulnerability assessments, log analysis, and malware behavior profiling.*
