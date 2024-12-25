# XtreamUIAccountTelegramManagerBot
  Manage xtreamui iptv users through telegram bot. Users can earn points through daily check-in through telegram bot and use the points to independently register accounts and choose packages to create their own iptv subscription links.

### How to

Create your telegram bot through botfather and record the token

Submit the following command to your bot

1. `/start`, `/help`: start using bot
2. `/info`: show user infos: points, status, account, expired date
3. `/traffic`: show server infos: online offline streaming etc.
4. `/checkin`: checkin for points
5. `/open_account`: open account using points
6. `/redeem_code`: redeem code
7. `/ban`: ban user, admin only
8. `/generate_code`: generate gift code, admin only




git clone https://github.com/qupaif/XtreamUIAccountTelegramManagerBot.git
pip install -r requeirments.txt
python3 main.py
