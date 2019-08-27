# wmurgu
It doesn't recognize myconfig.yml
- [x] I have searched for other issues with the same problem or similar feature requests. 

#### Select one:
- [x] Bug
- [ ] Feature Request
- [ ] Technical Help (Please don't create an issue, join the facebook group or telegram channel)
- [ ] Other

#### Environment
- [ ] Are you hosting the bot on a VPS or other Cloud hosting?
- [ ] Are you running the code on your phone 
- [x] If so, have you tried running the code on your local machine?

```
Include more details about the environment
```

#### Operating System? (include version)
- [ ] macOS
- [ ] Windows
- [ ] Rasbian Linux Raspberry PI (include flavour)
- [x] Linux (include flavour)
- [ ] Android (include terminal)

```
Linux subsystem on windows 4.4.0
```

#### Python Version Requirement
- [x] I am using Python 3.6 or above

#### Exact Python Version?
```
python 3.7.4
```

#### Pip Version?
```
pip 19.2.3
```

#### Instabot Version?
```
0.6.0
```

#### How you use the instabot
- [x] instabot-py -c my-configfile.yml (my-configfile.yml is an example you may have a different file )
- [ ] instabot-py --login LOGIN --password PASSWORD
- [ ] instabot-py 
- [ ] example.py (Deprecated, please install newer version) 


#### Description of your issue

```
I'm trying to pair it with myconfig.yml but it still run with its basic config. It doesn't recognize myconfig.yml
```

#### Config

```
Welcome to Neo-Instabot

THIS PROJECT HAS BEEN FORKED FROM neo-instabot Project.
DUE TO THE INACTIVITY OF ITS OWNER.

We hope that you enjoy the newer project.
Please follow & star the Neo-Instabot
Github : https://github.com/yurilaaziz/neo-instabot/
Telegram channel : https://t.me/joinchat/NTpLCxe7JqimNaZJYMRkYQ

Neo-Instabot is free and will remain free

login : "-----"
password : "-----"
accept_language: en-US,en;q=0.5
ban_sleep_time: 10800
comment_list:
- - this
  - the
  - your
- - photo
  - picture
  - pic
  - shot
  - snapshot
- - is
  - looks
  - feels
  - is really
- - great
  - super
  - good
  - very good
  - good
  - wow
  - WOW
  - cool
  - GREAT
  - magnificent
  - magical
  - very cool
  - stylish
  - beautiful
  - so beautiful
  - so stylish
  - so professional
  - lovely
  - so lovely
  - very lovely
  - glorious
  - so glorious
  - very glorious
  - adorable
  - excellent
  - amazing
- - .
  - ..
  - '...'
  - '!'
  - '!!'
  - '!!!'
comments_per_day: 0
comments_per_run: '{{comments_per_day}}'
config:
  file: instabot.config.yml
database:
  connection_string: sqlite:///{{database.path}}
  path: '{{login}}.db'
  type: sql
debug: 0
end_at_h: 23
end_at_m: 59
error_400_to_ban: 3
follow_per_day: 0
follow_per_run: '{{follow_per_day}}'
follow_time: 18000
follow_time_enabled: true
like_per_day: 1000
like_per_run: '{{like_per_day}}'
list_of_ua:
- Mozilla/4.0 (compatible; MSIE 6.0; Windows NT 5.1; FSL 7.0.6.01001)
- Mozilla/4.0 (compatible; MSIE 6.0; Windows NT 5.1; FSL 7.0.7.01001)
- Mozilla/4.0 (compatible; MSIE 6.0; Windows NT 5.1; FSL 7.0.5.01003)
- Mozilla/5.0 (Windows NT 6.1; WOW64; rv:12.0) Gecko/20100101 Firefox/12.0
- Mozilla/5.0 (X11; U; Linux x86_64; de; rv:1.9.2.8) Gecko/20100723 Ubuntu/10.04 (lucid)
  Firefox/3.6.8
- Mozilla/5.0 (Windows NT 5.1; rv:13.0) Gecko/20100101 Firefox/13.0.1
- Mozilla/5.0 (Windows NT 6.1; WOW64; rv:11.0) Gecko/20100101 Firefox/11.0
- Mozilla/5.0 (X11; U; Linux x86_64; de; rv:1.9.2.8) Gecko/20100723 Ubuntu/10.04 (lucid)
  Firefox/3.6.8
- Mozilla/4.0 (compatible; MSIE 6.0; Windows NT 5.0; .NET CLR 1.0.3705)
- Mozilla/5.0 (compatible; MSIE 9.0; Windows NT 6.1; WOW64; Trident/5.0)
- Mozilla/4.0 (compatible; MSIE 7.0; Windows NT 5.1; Trident/4.0; .NET CLR 2.0.50727;
  .NET CLR 3.0.4506.2152; .NET CLR 3.5.30729)
- Opera/9.80 (Windows NT 5.1; U; en) Presto/2.10.289 Version/12.01
- Mozilla/4.0 (compatible; MSIE 7.0; Windows NT 5.1; SV1; .NET CLR 2.0.50727)
- Mozilla/5.0 (Windows NT 5.1; rv:5.0.1) Gecko/20100101 Firefox/5.0.1
- Mozilla/5.0 (Windows NT 6.1; rv:5.0) Gecko/20100101 Firefox/5.02
- Mozilla/5.0 (Windows NT 6.0) AppleWebKit/535.1 (KHTML, like Gecko) Chrome/13.0.782.112
  Safari/535.1
- Mozilla/4.0 (compatible; MSIE 6.0; MSIE 5.5; Windows NT 5.0) Opera 7.02 Bork-edition
  [en]
logging:
  disable_existing_loggers: false
  formatters:
    simple:
      format: '%(asctime)s - {{login}} - %(name)s - %(levelname)s - %(message)s'
  handlers:
    console:
      class: logging.StreamHandler
      formatter: simple
      level: DEBUG
      stream: ext://sys.stdout
  loggers:
    InstaBot:
      handlers:
      - console
      level: WARN
      propagate: 'no'
    Persistence:
      handlers:
      - console
      level: WARN
      propagate: 'no'
  root:
    level: INFO
  version: 1
max_like_for_one_tag: 5
media_max_like: 150
media_min_like: 0
proxies:
  http: '{{ proxy_http_string if (proxy_ip and proxy_port)}}'
  https: '{{ proxy_http_string if (proxy_ip and proxy_port)}}'
proxy_auth: '{{ proxy_auth_string if (proxy_user and proxy_password)}}'
proxy_auth_string: '{{ proxy_user}}:{{proxy_password}}@'
proxy_http_string: http://{{proxy_auth}}{{proxy_ip}}:{{proxy_port}}
proxy_https_string: https://{{proxy_auth}}{{proxy_ip}}:{{proxy_port}}
session_file: '{{login}}.session'
start_at_h: 0
start_at_m: 0
tag_blacklist: []
tag_list:
- man
- bro
- bug
time_till_unlike: 259200
unfollow_break_max: 30
unfollow_break_min: 15
unfollow_everyone: false
unfollow_inactive: true
unfollow_not_following: true
unfollow_per_day: 0
unfollow_per_run: '{{unfollow_per_day}}'
unfollow_probably_fake: true
unfollow_recent_feed: true
unfollow_selebgram: false
unfollow_whitelist: []
unlike_per_day: 0
unlike_per_run: '{{unlike_per_day}}'
unwanted_username_list: []
user_blacklist: {}
user_max_follow: 0
user_min_follow: 0
window_check_every: 300



```
