# XtreamUIAccountTelegramManagerBot
	anage xtreamui iptv users through telegram bot. Users can earn points through daily check-in through telegram bot and use the points to independently register accounts and choose packages to create their own iptv subscription links.
### Telegram bot support commands:

1. `/start`, `/help`: start using bot
2. `/info`: show user infos: points, status, account, expired date
3. `/traffic`: show server infos: online offline streaming etc.
4. `/checkin`: checkin for points
5. `/open_account`: open account using points
6. `/redeem_code`: redeem code
7. `/ban`: ban user, admin only
8. `/generate_code`: generate gift code, admin only

### support features:

1. above commands
2. auto ban expired accounts

### mysql schema

| table          | domains                                                                                                                    |
|----------------|----------------------------------------------------------------------------------------------------------------------------|
| user_accounts  | user_id, tg_username, total_points, user_type, user_status, iptv_link, account_expired_time, last_checkin_time, user_extra |
| action_history | user_id, action_time, action_type, point_delta, now_points, action_extra                                                   | 
| gift_code      | code, contain_points, code_status, generate_time, code_expired_time, batch_id, generate_user, used_user, code_extra        |
| schedule_job   | job_id, job_status, job_type, job_creat_time, job_execute_time, job_extra                                                  |

user_type: admin, operator, user, blocked
user_status: guest, member, expired, blocked
code_status: unused, used, expired, blocked

### How to

