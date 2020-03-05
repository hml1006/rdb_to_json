# rdb_to_json
This script comes from python rdbtools cli command, because rdbtools JSONCallback 
would't convert utf8 chars printable, so this script rewrite JSONCallback.
Otherwise, this script has the same command line parameters with rdbtools cli.

## Install dependences
``` bash
pip install rdbtools python-lzf
```

## Usage
``` bash
$ ./rdb_to_json.py -c json --key "conf*" ./dump7379.rdb 
[{
"conf:1122330000050:dcs_info":{"conf_start_time":"2018/02/27 12:30:25","dcs_start_time":"2018/02/27 12:30:25","dcs_mode_start_time":"2018/02/27 12:30:25","dcs_mode":"free"},
"conf:1234560000511:live":{"live_name":"测试直播","live_start_time":"2018-2-9 12:30:20","max_user_time":"2018/02/09 13:30:20","max_user_count":"100","star":"4.5"},
"conf:1122330000051:dcs_info":{"conf_start_time":"2018/02/27 12:30:25","dcs_start_time":"2018/02/27 12:30:25","dcs_mode_start_time":"2018/02/27 12:30:25","dcs_mode":"free"},
"conf:1234560000511:dcs_info":{"conf_start_time":"2018/02/06 13:30:31","dcs_start_time":"2018/02/06 13:30:31","dcs_mode":"free","dcs_mode_start_time":"2018/02/06 13:30:31"}}]
```
