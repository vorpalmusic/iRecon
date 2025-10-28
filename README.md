<img width="687" height="207" alt="lantern-logo-color" src="https://github.com/user-attachments/assets/c7d56e1d-e62a-490a-b19b-6cc3e1e87ecb" />


Lantern began as a fork of a small nmap wrapper called iRecon ("an automated Nmap-based reconnaissance script designed to speed up the initial enumeration phase during CTFs or real-world pentests"). That script is small but was apparently the inspiration I needed. I envison 'lantern' now as a kind of external "linpeas"--for intitial information gathering in a pentest.

Find the original iRecon repo here--this little script inspired the current work: https://github.com/gzzcoo/iRecon

the README will be totally reworked to reflect the current project soon.

## Installation
Prerequisites
```bash
sudo apt install nmap xsltproc python3 wget bat firefox-esr lolcat xclip -y
```
Installing the tool
```bash
wget https://raw.githubusercontent.com/Gzzcoo/iRecon/refs/heads/main/iRecon
chmod +x iRecon
sudo mv iRecon /usr/local/bin/iRecon
```

## Usage
```bash
iRecon <IP>
```

## 🚀 Features

  - Performs a full port scan (-p-) using Nmap to detect open ports.

  - Automatically extracts open ports and copies them to your clipboard.

  - Detects service versions and runs basic reconnaissance scripts (-sCV) on discovered ports.

  - Generates a full Nmap XML report, transforms it into HTML, and opens it in your browser automatically.

  - Temporarily hosts the report using Python's HTTP server and releases the port right after.

  - Clean, quiet execution with colored terminal output (if added to your .zshrc or bash script).

## 📌 Why use iRecon?

While iRecon runs in the background automating tedious steps, you can focus on exploring services, web apps, or other vectors in parallel. This workflow dramatically reduces downtime and boosts productivity during reconnaissance.
No more wasting time typing repetitive Nmap commands or organizing reports manually — iRecon takes care of it all, and your port 6969 stays clean and free afterward 😉

## 🛠️ Perfect For

 
## 📸 Preview

