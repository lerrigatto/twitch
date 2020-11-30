# SRE live! Wireguard and SSHd - 20-11-30

Today's plan:

1 - Configure wireguard on my debian nas
2 - Ensure I can access that thing from the outside
3 - ...

Openssh server (default conf)
1) installing ssh on ym server
  apt install openssh-server
2) adding my pubkey
  wget https://github.com/lerrigatto.keys
  move that file on ~/.ssh/authorized_keys
3) add authorized keys conf option in sshd
4) Disable rootlogin, passwordauth, emptypasswords, X11forwarding
4) restarted sshd

Wireguard
1) install wireguard apt package
2) Create a wg0 wireguard interface
3) Assign ipv4 subnet to that interface
4) create a wg private and public keypair
5) setup wg0 with such key
6) Add postUp and PostDown commands for ipv4 forwarding
7) Open the wireguard port on your firewall
6) Create client conf (on clients)
7) Add peer conf to server
8) Create qrcode and setup android
9) Check if client internet connection works


TODO next:
- Run ansible playbooks against this server
- Configure sshd and wireguard trough ansible
- Update dns with current public ip of server
