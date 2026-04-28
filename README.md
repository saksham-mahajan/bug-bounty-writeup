# 👨‍💻 Cybersecurity Portfolio

Hi, I'm Saksham, a cybersecurity enthusiast focused on web application security and bug bounty.

## 🔍 Skills
- Web Application Testing
- Burp Suite
- Authentication Testing
- Vulnerability Analysis

## 📂 Writeups

### 🔐 OTP Rate Limiting Weakness 

#### Summary
Identified a weakness in OTP verification where the system allowed ~120–130 attempts before mitigation.

#### Methodology
- Intercepted OTP request using Burp Suite
- Used Intruder for controlled testing
- Observed response patterns

#### Findings
- 401 responses for multiple attempts
- Delayed mitigation (403 / CAPTCHA)
- No early lockout

#### Impact
- 4-digit OTP = 10,000 combinations
- ~130 attempts = ~1.3% coverage
- Increased brute-force feasibility


#### Tools Used
- Burp Suite
