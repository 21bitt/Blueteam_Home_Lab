
# Day 0 – Baseline Network

- ISP: T-Mobile 5G Home
- Gateway: UniFi Cloud Gateway Ultra
- Switch: UniFi Switch Ultra
- AP: U7 Lite
- Topology: Double NAT (ISP router upstream)

# Network Toplogy (Physical)
Internet

│

T-Mobile 5G Modem / Router / AP

│

UniFi Cloud Gateway Ultra (WAN)

│

UniFi Switch Ultra
  
  ├── AP7 Lite
  
  └── Custom PC


# Purpose:
- Establish known-good baseline before segmentation and monitoring

# Confirmed:
- Unifi UI is showing all the connected devices including my first host machine, custom pc.
- devices are up to date.
- no connection to unifi cloud. all localized.

-----------------------------------------------------------

# Day 1 - VLAN

-created first vlan with /28 mask and enabled the option to isolate this network using firewall rules.\
 -assigned VLAN 10 to AP7 Lite so private home wifi network (2.4ghz and 5ghz) is enabled. Security is WPA2/WPA3

*Error number 1. 
- Using my phone, connected to new wifi ssid established with VLAN 10 and AP7 Lite.
- The device received new ip address with accurate subnet mask. DNS is automatic. Yet no wifi traffic. 
