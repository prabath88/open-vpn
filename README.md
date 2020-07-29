# open-vpn configuration

Launch an EC2 instance on aws in the sublic subnet and follow the below steps to configure the client to site vpn.

sudo apt update
sudo apt upgrade -y
git clone https://github.com/prabath88/open-vpn.git

cd open-vpn
sudo chmod +x openvpn-install.sh
sudo ./openvpn-install.sh

Welcome to this OpenVPN road warrior installer!

Which IPv4 address should be used?
     1) 3.70.4.83
IPv4 address [1]:

Press enter

select the following options to complete the installation

1) public IP
2) UDP
3) Current system resolvers
4) clinet name
Note:- UDP is faster than TCP

Create users

sudo ./openvpn-install.sh

OpenVPN is already installed.

Select an option:
   1) Add a new client
   2) Revoke an existing client
   3) Remove OpenVPN
   4) Exit
Option:user1

Press enter

copy the user1.ovpn file to the client machine and use openvpn client to connect to the VPN server.



