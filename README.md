# RK322X Armbian Home Server

This project is intended to be a personal challenge, as well as a step by step guide for those who are interested in building a low-energy, fully-fledged domestic server

## Hadware Stack

We'll be using:
- **Nodes:** 3x MXQ Pro TV Boxes (Rockchip RK322x - 1GB RAM / 8GB eMMC)
- **Network:** 1x Intelbras SF 800Q+ FastEthernet Switch
- **Storage**: 1x Generic Sata M/M USB 3.0 Adapter and 1x Samsung 2.5" 1TB HDD
- **Gateway:** 1x Archer C3 Domestic Router 

Despite the high targeted software goal, the hardware will be simplified to things I already have at home, or cheap devices/tools I can easily find locally

## Architecture and Goals

Armbian - Well documented for Rockchip CPUs
Nginx - Integration with TV's Kodi App / Easy file sharing within devices
Docker - Docker Swarm for Cluster integration / Easy service and software management 
Torsocks - Will be used as a VPN despite low speed
Tailscale - Opening to the Internet
Pi-Hole - Ad-blocking in LAN
Nginx Proxy Manager - Reverse Proxying the Network
ModSecurity - WAF
Authelia - Authentication Manager
Jellyfin - Content Streaming
Jellyseer - Content Management
Nextcloud - Cloud Sevrices
Synthing - Synchronization Services
ELK Stack + Snort/Suricata - SIEM with IDS/IPS Monitoring
Gitea - Project Versioning
Aria2ng - Download Manager
QBittorrent - Torrent Manager
Iptables - Firewall
Prometheus+Grafana/Netdata - Metrics gathering
ClamAV - Heuristic and Signature based Antivirus
Lynis - Compliance and System Configuration auditor
Wireshark - Packet analyzer
FTP + SMB + SSH - Basic management services
Heimall - Dashboarding
Restic - Backup Services

If one or more services are not possible for network or hardware limitation, I'll make my own

Concerning security and learning, I'll also report any attempted Pentests against the server by me or my friends on this guide
