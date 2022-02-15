# VPN

◻️ `apt install openvpn -y` ;

◻️ `cd /etc/openvpn/` ;

◻️ `openvpn --genkey --secret ta.key` ;

◻️ `openssl dhparam -out dh2048.pem 2048` .

### After adding "server_ss.conf" and "server_ra.conf"

◻️ `systemctl enable --now openvpn@server_ss` ;

◻️ `systemctl enable --now openvpn@server_ra` ;

◻️ `systemctl restart openvpn@server_ss` ;

◻️ `systemctl restart --now openvpn@server_ra` ;

◻️ `systemctl status --now openvpn@server_ss` ;

◻️ `systemctl status openvpn@server_ra` .
