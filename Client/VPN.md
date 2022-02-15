# VPN

◻️ `apt install openvpn -y` ;

◻️ `cd /etc/openvpn/` ;

◻️ `nano ta.key` (copy ta.key from control.inova.pt) .

### After adding "client.conf" and "client2.conf"

◻️ `systemctl enable --now openvpn@client2` ;

◻️ `systemctl enable --now openvpn@client` ;

◻️ `systemctl restart openvpn@client2` ;

◻️ `systemctl restart --now openvpn@client` ;

◻️ `systemctl status --now openvpn@client2` ;

◻️ `systemctl status openvpn@client` ;
