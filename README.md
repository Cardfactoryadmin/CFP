<h1 align="center">CFPhisher</h1>

<p align="center">
  <img src="https://img.shields.io/badge/Version-2.1.7-green?style=for-the-badge">
  <img src="https://img.shields.io/github/stars/CardFactory/CFPhisher?style=for-the-badge&color=orange">
  <img src="https://img.shields.io/github/forks/CardFactory/CFPhisher?color=cyan&style=for-the-badge&color=purple">
  <img src="https://img.shields.io/github/watchers/CardFactory/CFPhisher?color=cyan&style=for-the-badge&color=purple">
  <img src="https://img.shields.io/github/issues/CardFactory/CFPhisher?color=red&style=for-the-badge">
  <img src="https://img.shields.io/github/license/CardFactory/CFPhisher?style=for-the-badge&color=blue">
  <img src="https://hits.dwyl.com/CardFactory/CFPhisher.svg" width="140" height="28">
<br>
<br>
  <img src="https://img.shields.io/badge/Author-CardFactory-purple?style=flat-square">
  <img src="https://img.shields.io/badge/Open%20Source-Yes-cyan?style=flat-square">
  <img src="https://img.shields.io/badge/Made%20in-UK-green?colorA=%23ff0000&colorB=%23017e40&style=flat-square">
  <img src="https://img.shields.io/badge/Written%20In-Python-blue?style=flat-square">
</p>


### [√] Description :

***Ultimate phishing tool in python. Includes popular websites like facebook, twitter, instagram, github, reddit, gmail and many others.***

### [*]Announcement

This project is now a part of [MaxPhisher](https://github.com/KasRoudra/MaxPhisher). Further bug fixes and feature addition will be available in that


### [+] Installation

##### Install dependencies (git, python, php ssh)

 - For Debian (Ubuntu, Kali-Linux, Parrot)
    - ```sudo apt install git python3 python3-pip php openssh-client -y```
 - For Arch (Manjaro)
    - ```sudo pacman -S git python3 python-pip php openssh --noconfirm```
 - For Redhat(Fedora)
    - ```sudo dnf install git python3 php openssh -y```
 - For Termux
    - ```pkg install git python3 python-pip php openssh -y```

##### Clone this repository

 - ```git clone https://github.com/Cardfactoryadmin/CFPhisher```

##### Enter the directory
 - ```cd CFPhisher```

##### Install all modules
 - ```pip3 install -r files/requirements.txt --break-system-packages```

##### Run the tool
 - ```python3 cfphisher.py```

#### Or, directly run
```
wget https://raw.githubusercontent.com/CardFactory/CFPhisher/main/CFPhisher.py && python3 CFPhisher.py

```

### Pip
 - `pip3 install CFPhisher` [For Termux]
 - `sudo pip3 install CFPhisher  --break-system-packages` [For Linux]
 - `CFPhisher`

### Docker

 - `sudo docker pull CardFactory/CFPhisher`
 - `sudo docker run --rm -it CardFactory/CFPhisher`

### Support

OS         | Support Level
-----------|--------------
Linux      | Excellent
Android    | Excellent
iPhone     | Alpha (Recommended docker)
MacOS      | Alpha (Recommended docker)
Windows    | Unsupported (Use docker/virtual-box/vmware)
BSD        | Never tested

#### Options

```
usage: CFPhisher.py [-h] [-p PORT] [-o OPTION] [-t TUNNELER]
                    [-r REGION] [-s SUBDOMAIN] [-u URL] [-m MODE]
                    [-e TROUBLESHOOT] [--nokey] [--noupdate]

options:
  -h, --help            show this help message and exit
  -p PORT, --port PORT  CFPhisher's server port [Default : 8080]
  -o OPTION, --option OPTION
                        CFPhisher's template index [Default : null]
  -t TUNNELER, --tunneler TUNNELER
                        Tunneler to be chosen while url shortening
                        [Default : Cloudflared]
  -r REGION, --region REGION
                        Region for loclx [Default: auto]
  -s SUBDOMAIN, --subdomain SUBDOMAIN
                        Subdomain for loclx [Pro Account]
                        (Default: null)
  -u URL, --url URL     Redirection url after data capture [Default :
                        null]
  -m MODE, --mode MODE  Mode of CFPhisher [Default: normal]
  -e TROUBLESHOOT, --troubleshoot TROUBLESHOOT
                        Troubleshoot a tunneler [Default: null]
  --nokey               Use localtunnel without ssh key [Default:
                        False]
  --noupdate            Skip update checking [Default : False]
```

### Features:

 - Multi platform (Supports most linux)
 - Easy to use
 - Possible error diagnoser
 - 77 Website templates
 - Concurrent 4 tunneling (Cloudflared, Loclx and LocalHostRun, Serveo)
 - Upto 8 links for phishing
 - OTP Support
 - Argument support
 - Credentials mailing
 - Built-in masking of URL
 - Custom masking of URL
 - URL Shadowing
 - Redirection URL settings
 - Portable file (Can be run from any directory)
 - Get IP Address and many other details along with login credentials

#### Relevant Tools by Me
 - [CamHacker](https://github.com/Cardfactoryadmin/CamHacker) for image phishing
 - [VidPhisher](https://github.com/Cardfactoryadmin/VidPhisher) for video phishing


### Requirements

 - `Python(3)`
   - `requests`
   - `rich`
   - `beautifulsoup4`
 - `PHP`
 - `SSH`
 - 900MB storage
 
If not found, php and python modoules will be installed on first run

#### Tested on

 - `Termux`
 - `Ubuntu`
 - `Kali-Linux`
 - `Arch`
 - `Fedora`
 - `Manjaro`

## Usage

1. Run the script
2. Choose a Website
3. Wait sometimes for setting up all
4. Send the generated link to victim
5. Wait for victim login. As soon as he/she logs in, credentials will be captured

<h1 align="center">Example</h1>

![CFPhisher](https://raw.githubusercontent.com/CardFactory/CFPhisher/main/files/cfphisher.gif)

## Video Tutorial
<a href="https://rebrand.ly/CFPhishervideo">CFPhisher in Termux</a>
<br/>
<a href="https://youtu.be/xIEuJkmJ8F0">CFPhisher in Kali Linux by InfoSecPat</a>
<br/>
<a href="https://youtu.be/ueF6fNHD8MM">CFPhisher in Kali Linux by Sathvik</a>

## Whats new in 1.8?
 - *Mailing*
   - Now you can send credentials to any email. You just need a gmail and app password to use this feature. Edit the data in `files/email.json`
 - *Custom Preview*
   - Now you can set a custom social media preview of your link. Enter a website url when asked in `shadow url`. Your link will have same appearence as that website in whatsapp/messenger/telegram etc. Note this only works with Cloudflared urls
 - *OTP Support*
   - 20 templates will show an option to enable otp pages
 - *Saved*
   - An option to view all saved credentials just from CFPhisher. This credentials won't get deleted in CFPhisher update

## Whats new in 1.9?
 - *Loclx*
   - Introducing a new port forwarding/tunneling service named localxpose or loclx. It is quite slower but still usable
 - *Docker image*
   - A docker image is published which can be pulled and run
 - *PIP*
   - This project is now also available in PIP

## Whats new in 2.0?
 - *LocalHostRun*
   - Introducing a new port forwarding/tunneling service named localhost.run. It works over ssh without binaries
 - *Redirection url*
   - Users can decide where the victim will be redirected after data is captured

## Solution of common issues
 - Some secured browsers like Firefox can warn for '@' prefixed links. You should use pure links or custom link to avoid it.
 - Termux from play store in not supported. Download termux from fdroid or github
 - VPN or proxy prevents tunneling and even proper internet access. Turn them off you have issues.
 - Some android requires hotspot to start Cloudflared and Loclx. If you face 'tunneling failed' in android, most probably your hotspot is turned off. Turn it on and keep it on untill you close CFPhisher.
 - If you want mailing credentials then you need to use app password. Visit [here](https://myaccount.google.com/u/0/apppasswords) and generate an app password, put that in `files/email.json`. You may need to enable 2FA before it.
 
## [!] Disclaimer
***This tool is developed for educational purposes. Here it demonstrates how phishing works. If anybody wants to gain unauthorized access to someones social media, he/she may try out this at his/her own risk. You have your own responsibilities and you are liable to any damage or violation of laws by this tool. The author is not responsible for any misuse of CFPhisher!***

### This repository is open source to help others. So if you wish to copy, consider giving credit!

## Credits:
Some base codes and templates are from [htr-tech](https://github.com/htr-tech/zphisher), otp templates are from [ignitech](https://guthub.com/ignitech/AdvPhishing) and url masking is inspired from [jaykali](https://github.com/jaykali/maskphish)


### [*] Support
####  Want to show support? Just spread the word and smash the star button
###### Donate BTC: ***3Lx8ikQQgZZpmFJzHDBuQHXzLXMeWMcZF3***

## [~] Find Me on :

- [![Github](https://img.shields.io/badge/Github-CardFactory-purple?style=for-the-badge&logo=github)](https://github.com/Cardfactoryadmin)

- [![Gmail](https://img.shields.io/badge/Gmail-CardFactory-green?style=for-the-badge&logo=gmail)](mailto:Crdfctry@gmail.com)

- [![Facebook](https://img.shields.io/badge/Facebook-CardFactory-blue?style=for-the-badge&logo=facebook)](https://facebook.com/CardFactory)

- [![Messenger](https://img.shields.io/badge/Messenger-CardFactory-orange?style=for-the-badge&logo=messenger)](https://m.me/CardFactory)

- [![Telegram](https://img.shields.io/badge/Telegram-CardFactory-indigo?style=for-the-badge&logo=telegram)](https://t.me/cardfactoryadmin)

