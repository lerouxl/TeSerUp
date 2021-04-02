# TardisLink

## Goal:
Send telegram update from my serveur to a Telegram chanel.
Idea from https://dev.to/bogkonstantin/send-message-to-telegram-on-any-ssh-login-24c8 and https://github.com/NicolasBernaerts/debian-scripts/tree/master/telegram 

## Setup:
- Install telegram script from [Nicolas Bernaerts](https://github.com/NicolasBernaerts/debian-scripts/tree/master/telegram): 
	- `wget https://raw.githubusercontent.com/NicolasBernaerts/debian-scripts/master/telegram/telegram-notify-install.sh`
	- `chmod +x telegram-notify-install.sh`
	- `sudo ./telegram-notify-install.sh`
- Set your api-key and user/chanel id  in /etc/telegram-notify.conf:
	- `sudo nano /etc/telegram-notify.conf`
	- test with `telegram-notify --text "test msg"`
- Make telegram-login-msg.sh usable and move it:
	- `chmod +x telegram-login-msg.sh`
	- 'sudo cp telegram-login-msg.sh /etc/profile.d/telegram-login-msg.sh' 



