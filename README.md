# ids_alert
It gives a visual alert on suricata and snort in a cause of intrution and asks you to disable the internet or not.


How to run it:
        pip3 install -r requiremnts.txt && sudo apt install mpg123 -y  #plus you need mpg123 for the notification sound
        python3 ids_alert.py > /dev/null 2>&1 &
        # or you can put it in crontab or something like that ;)

WARNING:
        Be carefull with configuration of snort and suricata cause this script is checking the alert logs and if detect's a change its going to print the last line in case of massive attack (like ddos,portscan etc.) so it might generate false positives alerts.
        
        This script was done in 2 days so it's a bit shitty written but you can take it and modify it in your way :)
