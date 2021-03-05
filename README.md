# Ansible-Scripts

## Wireguard - wireguard.yml (Initialize wireguard)
```
sudo ansible-playbook -e "ip_addr={VPN ip address for this device(i.e. 10.10.10.1/24)} interface={interface for vpn(i.e. eth0)}" wireguard.yml
```
#### Example
```
sudo ansible-playbook -e "ip_addr=10.10.10.1/24 interface=eth0" wireguard.yml
```
<br />


### Wireguard - wireguard-peer.yml (Add peer)
```
sudo ansible-playbook -e "user={peer username (i.e. mixalis)}" wireguard-peer.yml
```
#### Example
```
sudo ansible-playbook -e "user=trixas97" wireguard-peer.yml
```


### Wireguard - wireguard-peer-revoke.yml (Revoke peer)
```
sudo ansible-playbook -e "user={peer username (i.e. mixalis)} revoke={yes or no}" wireguard-peer-revoke.yml
```
#### Example
```
sudo ansible-playbook -e "user=trixas97 revoke=yes" wireguard-peer-revoke.yml
```


### Wireguard - wireguard-peer-remove.yml (Remove peer)
```
sudo ansible-playbook -e "user={peer username (i.e. mixalis)}" wireguard-peer-remove.yml
```
#### Example
```
sudo ansible-playbook -e "user=trixas97" wireguard-peer-remove.yml
```
