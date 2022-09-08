# Cisco-VPN-cheatSheet

This repo describes the configuration of various Cisco VPN solutions

## Quick navigation

- [VPN Site To Site Preshared Key Auth](README.md#VPN-Site-To-Site-Preshared-Key-Auth)
- [VPN Site To Site Certificate-Based](README.md#VPN-Site-To-Site-Certificate-Based)
- [DMVPN Phase 1](README.md#DMVPN-Phase-1)
- [DMVPN Phase 2](README.md#DMVPN-Phase-2)
- [DMVPN Phase 3](README.md#DMVPN-Phase-3)
- [Dynamic VTI ](README.md#Dynamic-VTI)
- [GetVPN Single Hub](README.md#GetVPN-Single-Hub)
- [GetVPN Dual Hub](README.md#GetVPN-Dual-Hub)



## VPN Site To Site Preshared Key Auth
### Phase 1 configuration
```
crypto isakmp policy 1
   encr [encryption-Algorithm]
   hash [Hash-Algorithm]
authentication pre-share
group [Deffie-Hellman-Group]
lifetime [Seconds]
```


## VPN Site To Site Certificate-Based

### Prerequesite

- Time synchronisation NTP
- Active HTTP Server
#### CA Server 

- Define the domain name
 `ip domain-name domain.name`
- generate an exportable RSA Key
crypto key generate rsa modulus 1024 label `KEY_NAME` exportable

## DMVPN Phase 1
## DMVPN Phase 2
## DMVPN Phase 3
## Dynamic VTI
## GetVPN Single Hub
## GetVPN Dual Hub










