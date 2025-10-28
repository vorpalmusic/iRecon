<img width="687" height="207" alt="lantern-logo-color" src="https://github.com/user-attachments/assets/c7d56e1d-e62a-490a-b19b-6cc3e1e87ecb" />

Lantern began as a fork of a small nmap wrapper called iRecon ("an automated Nmap-based reconnaissance script designed to speed up the initial enumeration phase during CTFs or real-world pentests"). That script is small but was apparently the inspiration I needed. I envison 'lantern' now as a kind of external "linpeas"--for intitial information gathering in a pentest.

Find the original iRecon repo here--this little script inspired the current work: https://github.com/gzzcoo/iRecon

the README will be totally reworked to reflect the current project soon (today is Oct 29, 2025).

## Installation
Prerequisites (IN PROGRESS)
```bash
sudo apt install nmap xsltproc python3 wget bat firefox-esr lolcat xclip -y
```
Installing the tool
```bash
git clone https://github.com/vorpalmusic/lantern.git
sudo ln -sf ~/lantern/lantern /usr/local/bin/lantern
```

## Usage
```bash
lantern <IP>
```
The first run will generate prompts (TBD) allowing you to install the tool globally if desired, to change the web server port (default 9999), etc.

## 🚀 Features

  - Performs a full port scan (-p-) using Nmap to detect open ports.
  - Automatically extracts open ports and copies them to your clipboard.
  - Detects service versions and runs basic reconnaissance scripts (-sCV) on discovered ports.
  - Generates a full Nmap XML report, transforms it into HTML, and opens it in your browser automatically.
  - Temporarily hosts the report using Python's HTTP server.
  - Deep dive on all discovered services coming, so far HTTP in partial completion.

## 📌 Why use lantern?

While lantern runs in the background automating tedious steps, you can focus on exploring services, web apps, or other vectors in parallel. This workflow dramatically reduces downtime and boosts productivity during reconnaissance.
No more wasting time typing repetitive Nmap commands or organizing reports manually — lantern takes care of it all 😉

## 🛠️ Perfect For
pen-tests, red teaming and CTFs
