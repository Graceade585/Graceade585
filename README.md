- 👋 Hi, I’m @Graceade585
- 👀 I’m interested in ...
- 🌱 I’m currently learning ...
- 💞️ I’m looking to collaborate on ...
- 📫 How to reach me ...
- 😄 Pronouns: ...
- ⚡ Fun fact: ...

# Configure VPN server settings
server_ip = 'your_vpn_server_ip'
server_port = 1194
username = 'your_vpn_username'
password = 'your_vpn_password'

# Establish VPN connection
vpn = openvpn.OpenVPN()
vpn.connect(server_ip, server_port, username, password)

# Monitor and log connected users
def monitor_users(vpn):
    while True:
        users = vpn.get_connected_users()
        print("Connected users:", users)
        time.sleep(60)  # Check every minute

monitor_users(vpn)
<!---
Graceade585/Graceade585 is a ✨ special ✨ repository because its `README.md` (this file) appears on your GitHub profile.
You can click the Preview link to take a look at your changes.
--->
