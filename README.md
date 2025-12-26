install auto screen untuk sinyal jelek biar tersambung terus

```
sysctl -w net.ipv6.conf.all.disable_ipv6=1 && sysctl -w net.ipv6.conf.default.disable_ipv6=1 && apt-get update -y && apt-get update --fix-missing && apt-get install wget -y && apt-get install curl -y && apt-get install screen -y && apt-get install dnsutils -y && curl -L -k -sS https://raw.githubusercontent.com/mudziboy/tunv2/main/setup.sh -o rmck && chmod +x rmck && screen -S InstallAutoScript ./rmck; if [ $? -ne 0 ]; then rm -f rmck; fi
```
untuk update script

```wget -q -O /usr/bin/update "https://raw.githubusercontent.com/mudziboy/tunv2/main/update" && chmod +x /usr/bin/update && update```
