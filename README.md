asd
sudo   -i
apt update && apt install dnsmasq -y
cat << 'EOFC' >/etc/dnsmasq.conf
domain-needed
bogus-priv
no-resolv
server=/baidu.com/8.8.8.8

EOFC
https://rootexplorer.co/

下载reqable辅助服务
下载质感文件app或者termux把证书从
cp /storage/emulated/0/Download/Reqable/d52c80b9.0 /system/etc/security/cacerts/d52c80b9.0

 systemctl restart dnsmasq
 iptables -A OUTPUT -p udp --dport 53 -j ACCEPT
 iptables -A OUTPUT -p tcp -d  baidu.com_ip -j ACCEPT
 iptables -A OUTPUT -p udp -d baidu.com_ip -j ACCEPT
 iptables -P OUTPUT DROP
下面第二个扩展工具-全局打开root
