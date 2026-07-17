CyberrhodzUrlmask is an open-source URL masking and analysis tool designed for **security research, phishing awareness, and defensive testing**.  
It demonstrates how adversaries may disguise malicious links using URL manipulation and social engineering techniques, helping defenders understand and mitigate such attacks.

## 🧭 MITRE ATT&CK Mapping

![MITRE ATT&CK](https://img.shields.io/badge/MITRE%20ATT%26CK-T1665-blue)
![Tidal Cyber](https://img.shields.io/badge/Referenced%20by-Tidal%20Cyber-0aa2a2)

Mapped to **MITRE ATT&CK® T1665 – Hide Infrastructure (Command and Control)**.  
This project is publicly referenced by **Tidal Cyber (Community Edition)** as part of adversary behavior research.

🔗 https://app.tidalcyber.com/references/bd80f3d7-e653-5f8f-ba8a-00b8780ae935

> [!IMPORTANT]
> **Educational & Defensive Use Only**
>
> CyberrhodzUrlmask is a proof-of-concept project intended for **security research, phishing awareness training, and authorized penetration testing**.
> It demonstrates techniques used by real-world attackers so defenders can better recognize, detect, and prevent them.
>
> Unauthorized or malicious use is strictly discouraged.

### Run Online Free On Google Colab

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/spyboy-productions/Facad1ng/blob/main/Facad1ng.ipynb)

### Example:
```
Your phishing link: https://example.com/whatever

Give any custom URL: gmail.com

Phishing keyword: anything-u-want

Output: https://gamil.com-anything-u-want@tinyurl.com/yourlink

# Get 4 masked URLs like this from different URL-shortener 

```

---

### ⭔ Key Features:

- **URL Masking**: Facad1ng allows users to mask URLs with a custom domain and optional phishing keywords, making it difficult to identify the actual link.

- **Multiple URL Shorteners**: The tool supports multiple URL shorteners, providing flexibility in choosing the one that best suits your needs. Currently, it supports popular services like TinyURL, osdb, dagd, and clckru.

- **Input Validation**: Facad1ng includes robust input validation to ensure that URLs, custom domains, and phishing keywords meet the required criteria, preventing errors and enhancing security.

- **User-Friendly Interface**: Its simple and intuitive interface makes it accessible to both novice and experienced users, eliminating the need for complex command-line inputs.

- **Open Source**: Being an open-source project, Facad1ng is transparent and community-driven. Users can contribute to its development and suggest improvements.

---

<h4 align="center">
  OS compatibility :
  <br><br>
  <img src="https://img.shields.io/badge/Windows-05122A?style=for-the-badge&logo=windows">
  <img src="https://img.shields.io/badge/Linux-05122A?style=for-the-badge&logo=linux">
  <img src="https://img.shields.io/badge/Android-05122A?style=for-the-badge&logo=android">
  <img src="https://img.shields.io/badge/macOS-05122A?style=for-the-badge&logo=macos">
</h4>

<h4 align="center"> 
Requirements:
<br><br>
<img src="https://img.shields.io/badge/Python-05122A?style=for-the-badge&logo=python">
<img src="https://img.shields.io/badge/Git-05122A?style=for-the-badge&logo=git">
</h4>

### ⭔ Git Installation
---

```
git clone https://github.com/viper081599/cyberrhodzUrlmask.git
```
```
cd cyberrhodzUrlmask
```
```
pip3 install -r requirements.txt
```
```
python3 cyberrhodzUrlmask.py
```


### Python code:
```py
import subprocess

# Define the command to run your CyberrhodzUrlmask script with arguments
command = ["python3", "-m", "cyberrhodzurlmask.main", "https://ngrok.com", "facebook.com", "login"]

# Run the command
process = subprocess.Popen(command, stdout=subprocess.PIPE, stderr=subprocess.PIPE)

# Wait for the process to complete and get the output
stdout, stderr = process.communicate()

# Print the output and error (if any)
print("Output:")
print(stdout.decode())
print("Error:")
print(stderr.decode())

# Check the return code to see if the process was successful
if process.returncode == 0:
    print("cyberrhodzurlmask completed successfully.")
else:
    print("cyberrhodzurlmask encountered an error.")
```

---

## Contribution:

Contributions and feature requests are welcome! If you encounter any issues or have ideas for improvement, feel free to open an issue or submit a pull request.

#### 😴🥱😪💤 ToDo:

- Fix trycloudflare error which is blocked by TinyURL 

TinyURL not shorting trycloudflare
Solution: don’t use pyshortner. shorten links manually one by one if TinyURL blocks try using different shortener

#### 💬 If having an issue [Chat here] (https://web.facebook.com/search/top/?q=cyber%20rhodz)


<h4 align="center"> If you find this GitHub repo useful, please consider giving it a star! ⭐️ </h4> 
