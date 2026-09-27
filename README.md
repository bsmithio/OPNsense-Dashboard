No longer maintained by me. I have not been able to keep up with the updates as life circumstances have gotten in the way of this project. Please check out [tekgnosis-net/OPNsense-Dashboard](https://github.com/tekgnosis-net/OPNsense-Dashboard) for further updates.

# What's Monitored
- Active Users
- Uptime
- CPU Load total
- Disk Utilization
- Memory Utilization
- CPU Utilization per core (Single Graph)
- Ram Utilization time graph
- Load Average
- Load Average Graph
- CPU and ACPI Temperature Sensors
- Gateway Response time - dpinger
- List of interfaces with IPv4, IPv6, Subnet, MAC, Status and pfSense labels thanks to [/u/trumee](https://www.reddit.com/r/PFSENSE/comments/fsss8r/additional_grafana_dashboard/fmal0t6/)
- WAN Statistics - Traffic & Throughput (Identified by dashboard variable)
- LAN Statistics - Traffic & Throughput (Identified by dashboard variable)
- Firewall Statistics - Blocked Ports, Protocols, Events, Blocked IP Locations, and Top Blocked IP
# Changelog


Converted InfluxQL queries to Flux.

Converted pfSense functions to OPNsense.

Added Firewall panels.

Added subnet info to Interface Summary panels

Added Suricata dashboard, see instructions [here](./configure.md#configuration-for-the-suricata-dashboard-optional)

Added RFC5424 support thanks to [subract](https://github.com/IRQ10/Graylog-OPNsense_Extractors/pull/11)

![Main Dashboard](Grafana-OPNsense.png)

![Suricata Dashboard](Grafana-OPNsense-Suricata.png)

# Running on

    Grafana 9.2.10
    InfluxDB 2.6.1
    Graylog 5.0.2


# Configuration
Configuration instructions can be found [here](./configure.md).
