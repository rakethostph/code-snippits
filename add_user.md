# Adding User to Ubunto 18.04

`ssh root@your_server_ip`
Add User
`adduser username`

Enter Password
`passwd`

Add Sudo
`usermod -aG sudo username`
Add Firewall
```
ufw app list
ufw allow OpenSSH
ufw enable
ufw status
```
Change PasswordAuthentication from No to Yes

`nano /etc/ssh/sshd_config`
```
PasswordAuthentication no
# PasswordAuthentication yes
```
Restart server 
`sudo service ssh restart`

Copy ssh to the server

`ssh-copy-id username@your_server_ip`

then login
`ssh username@your_server_ip`
