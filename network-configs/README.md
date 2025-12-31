
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

