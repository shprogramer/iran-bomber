# iran-bomber
sms bomber pro irani 🇮🇷v1 with Go (Golang)
<img src="screen/Screenshot_20230815-000720_Chrome.jpg">

<h3>views :</h3>
<br>
<img src="https://profile-counter.glitch.me/esfelurm/count.svg" alt="Visitors">

## Number of web services 

- Sms : 177 🧨
- Call : 6 🧨

## Speed +

## Support from [tested]
- `Linux` ✅
- `Windows` ✅
- `Termux` ✅


## screen shot

<img src="screen/IMG_20230815_002517_499.png">

## prerequisite :

- Windows : Download Golang programming language from reputable sites

- Linux : `sudo apt install golang`

- Termux : `pkg install golang`

## Run in windows

`Enter the Windows folder and run the sms.exe file`

## Run in Linux/Termux

```
git clone https://github.com/esfelurm/iran-bomber
cd iran-bomber
go run sms.go
```
```
{                                                                         "route": {
                "geoip": {                                                        "path": "geo-assets\\sagernet-sing-geoip-geoip.db"
                },                                                                "geosite": {
                "path": "geo-assets\\sagernet-sing-geosite-geosite.db"
                },                                                                "rules": [
                {                                                                         "inbound": "dns-in",
                        "outbound": "dns-out"                                     },
                {                                                                         "port": 53,
                        "outbound": "dns-out"                                     },
                {                                                                         "clash_mode": "Direct",
                        "outbound": "direct"                                      },
                {                                                                         "clash_mode": "Global",
                        "outbound": "select"                                      }
                ],                                                                "auto_detect_interface": true,
                "override_android_vpn": true                              },
        "outbounds": [                                                            {
                "type": "selector",                                               "tag": "select",
                "outbounds": [                                                            "auto",
                        "IP->Iran, Yotube:Geekmeek",                                      "IP->Main, Yotube:Geekmeek"
                ],                                                                "default": "auto"
                },                                                                {
                "type": "urltest",                                                "tag": "auto",
                "outbounds": [
                        "IP->Iran, Yotube:Geekmeek",
                        "IP->Main, Yotube:Geekmeek"
                ],
                "url": "http://cp.cloudflare.com/",
                "interval": "10m0s"
                },
                {
                "type": "wireguard",
                "tag": "IP->Iran, Yotube:Geekmeek",
                "local_address": [
                        "172.16.0.2/32",
                        "2606:4700:110:80ff:fa5d:d116:b293:a01c/128"
                ],
                "private_key": "WO/sgYSgXiRg6nJR9M2/YkmV+CnTjdQ5A0qP3abazFo=",
                "server": "188.114.96.95",
                "server_port": 854,
                "peer_public_key": "bmXOC+F1FxEMF9dyiK2H5/1SUtzH0JuVo51h2wPfgyo=",
                "reserved": [41,231,116],
                "mtu": 1280,
                "fake_packets": "5-10"
                },
                {
                "type": "wireguard",
                "tag": "IP->Main, Yotube:Geekmeek",
                "detour": "IP->Iran, Yotube:Geekmeek",
                "local_address": [
                        "172.16.0.2/32",
                        "2606:4700:110:81be:6fe9:88e8:f6b:c1ab/128"
                ],
                "private_key": "KEjOTAHfgyTAFY8EgQ+SkPq++ZGdw8H2icz+9ROC6Gw=",
                "server": "188.114.96.95",
                "server_port": 854,
                "peer_public_key": "bmXOC+F1FxEMF9dyiK2H5/1SUtzH0JuVo51h2wPfgyo=",
                "reserved": [59,80,178],
                "mtu": 1280,
                "fake_packets": "5-10"
                },
                {
                "type": "dns",
                "tag": "dns-out"
                },
                {
                "type": "direct",
                "tag": "direct"
                },
                {
                "type": "direct",
                "tag": "bypass"
                },
                {
                "type": "block",
                "tag": "block"
                }
        ]
        }
```
 Good bye
