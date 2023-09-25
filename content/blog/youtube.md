+++
title = "selfhosted youtube."
author = "aadi."
date = 2023-09-25
+++
youtube-local

<!-- more -->

[youtube-local](https://github.com/user234683/youtube-local) is really cool service that allows you to self host your own instance of youtube.

i have tried to install another popular self-hostable instance of youtube, a fork of this very project, [yt-local](https://git.sr.ht/~heckyel/yt-local) but unfortunately, was unable to make the video player work for some reason.

anyways regardless of that, it was very easy to install youtube-local on my system,

---
```sh
git clone https://github.com/user234683/youtube-local yt-local
cd yt-local

python3 -m venv env
source env/bin/activate
pip3 install -r requirements.txt

python3 server.py
```
---
making a .service file for systemd,

---
```yaml
[Unit]
Description=My Youtube
[Service]
ExecStart=/home/aadi/.local/src/yt-local/env/bin/python /home/aadi/.local/src/yt-local/server.py
Exec=/home/aadi/.local/src/yt-local/env/bin/python /home/aadi/.local/src/yt-local/server.py
ExecReload=/home/aadi/.local/src/yt-local/env/bin/python /home/aadi/.local/src/yt-local/server.py
```
---
and also setting up a redirect plugin to make everything youtube reroute to my instance of yt, using a firefox plugin called [redirector](https://addons.mozilla.org/en-US/firefox/addon/redirector/).

---
```
^(https?://(?:[a-zA-Z0-9_-]*\.)?(?:youtube\.com|youtu\.be|youtube-nocookie\.com)/.*)
```
---


im currently having fun using this as,
- its very smooth
- it allowed me to import my subscriptions from [newpipe](https://newpipe.net/)
- it allows for customisability



---
all that aside, im doing well, ive been studying hard :)
cyall <3 bai
