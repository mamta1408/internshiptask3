# internshiptask3

# 🛡️ Vulnerability Assessment Report

## 🎯 Objective:
Use free tools to identify common vulnerabilities on your computer.

## 🛠️ Tools Used:
- **Tenable Nessus Essentials** (Free Vulnerability Scanner)  
  *(Alternative Option: OpenVAS Community Edition)*

## 📦 Deliverables:
- ✅ Vulnerability scan report with identified issues
- ✅ Summary of key findings and recommendations
- ✅ Screenshot of scan results


---

# 📄 Vulnerability Scan Report - Localhost (`mamta1`)

**Scanner**: Tenable Nessus Essentials  
**Scan Policy**: Advanced Scan  
**Target**: Localhost  
**Scan Status**: ✅ Completed  
**Severity Base**: CVSS v3.0  
**Scanner Type**: Local Scanner  
**Start Time**: Today at 8:20 PM  
**End Time**: Today at 8:28 PM  
**Elapsed Time**: 7 minutes  
**Total Vulnerabilities Found**: 25

---

## 📊 Vulnerability Summary

| Severity | Count |
|----------|-------|
| 🔴 Critical | 0     |
| 🟠 High     | 1     |
| 🟡 Medium   | 1     |
| 🔵 Low      | 0     |
| ⚪ Info     | 23    |

> 🎯 **Note**: Most findings are informational. However, two require attention.

## 🚨 Top Vulnerabilities

### 1. **SMB Signing Not Required**
- **Severity**: Medium
- **CVSS Score**: 5.3
- **Family**: Misc.
- **Count**: 1
- **Description**: SMB Signing is not required, which may allow man-in-the-middle attacks.
- **Recommendation**: Enforce SMB signing to prevent unauthorized tampering with SMB traffic.

- 
---

## ℹ️ Informational Findings (Samples)

| Name                                      | Family           | Count |
|-------------------------------------------|------------------|-------|
| SMB (Multiple Issues)                     | Windows          | 5     |
| HTTP (Multiple Issues)                    | Web Servers      | 2     |
| Microsoft Windows (Multiple Issues)       | Windows          | 2     |
| TLS (Multiple Issues)                     | Service Detection| 2     |
| Netstat Portscanner (SSH)                 | Port Scanners    | 47    |
| DCE Services Enumeration                  | Windows          | 8     |
| Service Detection                         | Service Detection| 3     |
| Common Platform Enumeration (CPE)         | General          | 1     |

---

## 🔧 Recommendations

- **Enforce SMB signing** and apply latest security patches to avoid MITM attacks.
- **Harden SSL/TLS configurations** by disabling weak protocols and using modern cipher suites.
- **Review all informational alerts** — while not immediately dangerous, they help in attack surface mapping.
- **Restrict unnecessary open ports and services** based on port scanner results.

---

## 📸 Screenshot of Scan Results
<img width="1842" height="904" alt="image" src="https://github.com/user-attachments/assets/adb296d8-a0dc-4b6c-bc44-1aab650612f4" />



---

## 📚 References

- [SMB Signing Best Practices - Microsoft Docs](https://docs.microsoft.com/en-us/windows-server/security/windows-services/security-guidelines-for-smb)
- [TLS/SSL Configuration - OWASP Guide](https://owasp.org/www-project-top-ten/)

---

## 📝 Notes

- This scan was done on a local machine using Nessus Essentials.
- Further manual review may be required to validate vulnerability impact.
- Automated tools provide quick identification but human review is essential for final triage.

---

**Prepared by**: `mamta1`  
**Tool**: Tenable Nessus Essentials  
