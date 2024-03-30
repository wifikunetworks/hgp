```
opkg update && wget --no-check-certificate "https://raw.githubusercontent.com/wifikunetworks/hgp/main/autotimesync.sh" -O /usr/bin/autotimesync.sh && chmod +x /usr/bin/autotimesync.sh

wget --no-check-certificate https://install.speedtest.net/app/cli/ookla-speedtest-1.2.0-linux-aarch64.tgz -O /tmp/speedtest.tgz && tar -xzvf /tmp/speedtest.tgz -C /usr/bin/ && chmod +x /usr/bin/speedtest

wget --no-check-certificate -P /root https://github.com/wifikunetworks/hgp/raw/main/luci-app-tailscale_1.0.5_all.ipk && opkg install --force-overwrite /root/luci-*-tailscale*.ipk && rm /root/*.ipk

opkg install screen

wget --no-check-certificate -P /root https://raw.githubusercontent.com/wifikunetworks/hgp/main/luci-app-lite-watchdog_1.0.14-20240101_all.ipk && opkg install --force-overwrite /root/luci-*-watchdog*.ipk && rm /root/*.ipk

opkg remove --force-remove luci-app-zerotier && wget --no-check-certificate -P /root https://raw.githubusercontent.com/wifikunetworks/hgp/main/luci-app-zerotier_git-23.137.55137-42dce6a_all.ipk && opkg install --force-overwrite /root/luci-*-zerotier*.ipk && rm /root/*.ipk

opkg remove --force-remove luci-app-sms-tool-js && rm /etc/config/sms_tool_js && wget --no-check-certificate -P /root https://raw.githubusercontent.com/wifikunetworks/hgp/main/luci-app-sms-tool-js_2.0.20-20240201_all.ipk && opkg install --force-reinstall /root/luci-*-sms*.ipk && rm /root/*.ipk


wget -O /etc/profile.d/30-sysinfo.sh https://raw.githubusercontent.com/wifikunetworks/hgp/main/30-sysinfo.sh
wget -O /tmp/sysinfo/model https://raw.githubusercontent.com/wifikunetworks/hgp/main/model
wget -O /etc/banner https://raw.githubusercontent.com/wifikunetworks/hgp/main/banner
wget -O /etc/config/system https://raw.githubusercontent.com/wifikunetworks/hgp/main/system
wget -O /etc/config/wireless https://raw.githubusercontent.com/wifikunetworks/hgp/main/wireless
wget -O /etc/modem/atcommands.user https://raw.githubusercontent.com/wifikunetworks/hgp/main/atcommands.user
wget -O /etc/modem/atcmmds.user https://raw.githubusercontent.com/wifikunetworks/hgp/main/atcmmds.user
wget -O /etc/config/atcmds.user https://raw.githubusercontent.com/wifikunetworks/hgp/main/atcmds.user
wget -O /www/luci-static/material/brand.png https://raw.githubusercontent.com/wifikunetworks/hgp/main/brand.png
wget -O /www/luci-static/argon/brand.png https://raw.githubusercontent.com/wifikunetworks/hgp/main/brand.png
wget -O /etc/rc.local https://raw.githubusercontent.com/wifikunetworks/hgp/main/rc.local
wget -O /etc/crontabs/root https://raw.githubusercontent.com/wifikunetworks/hgp/main/root
wget -O /usr/bin/hgled https://raw.githubusercontent.com/wifikunetworks/hgp/main/hgled && chmod +x /usr/bin/hgled
wget -O - https://raw.githubusercontent.com/wifikunetworks/hgp/main/navbar.tar | tar -xf - -C /www/luci-static/argon/
wget -O /usr/lib/lua/luci/view/themes/argon/footer_login.htm https://raw.githubusercontent.com/wifikunetworks/hgp/main/footer_login.htm
wget -O /usr/lib/lua/luci/view/themes/argon/footer.htm https://raw.githubusercontent.com/wifikunetworks/hgp/main/footer.htm
wget -O /usr/lib/lua/luci/view/themes/argon/header.htm https://raw.githubusercontent.com/wifikunetworks/hgp/main/header.htm
wget -O  /usr/bin/lite_watchdog.sh https://raw.githubusercontent.com/wifikunetworks/hgp/main/lite_watchdog.sh && chmod +x /usr/bin/lite_watchdog.sh
```
