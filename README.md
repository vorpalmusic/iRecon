# iRecon 🧠⚡

iRecon is an automated Nmap-based reconnaissance script designed to speed up the initial enumeration phase during CTFs or real-world pentests. It's especially useful for platforms like Hack The Box, where time and efficiency are key.

## Installation
```bash
sudo apt install nmap xsltproc python3 wget batcat -y
```
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

  - Hack The Box

  - TryHackMe

  - Offensive Security Labs

  - Red Team internal recon

  - Any scenario where speed and output clarity matter

## 📸 Preview

![imagen](https://github.com/user-attachments/assets/04c5c804-669f-4714-9ab4-10453bf10659)


https://github.com/user-attachments/assets/a98b0c4b-a0da-4168-81d3-2bc8c72cf709

