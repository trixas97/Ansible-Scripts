# Ansible-Scripts
# vue-project

## Wireguard - wireguard.yml (Initialize wireguard)
```
sudo ansible-playbook -e "ip_addr={VPN ip address for this device(i.e. 10.10.10.1/24)} interface={interface for vpn(i.e. eth0)}" wireguard.yml
```
#### Example
```
sudo ansible-playbook -e "ip_addr=10.10.10.1/24 interface=eth0" wireguard.yml
```




### Wireguard - wireguard-peer.yml (Add peer to wireguard)
```
sudo ansible-playbook -e "user={peer username (i.e. mixalis)}" wireguard-peer.yml
```
#### Example
```
sudo ansible-playbook -e "user=trixas97" wireguard-peer.yml
```
