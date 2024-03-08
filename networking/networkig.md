# Networking
---

## Static Ip address (Ubuntu 20.04+, netplan)

```bash
# Open default netplan config file
sudo nano /etc/netplan/01-network-manager-all.yaml

# Figure out network details
ip route

# Example output
# There might be other lines only the ones with the same interface as default matters
default via 192.168.1.254 dev wlp4s0 proto dhcp src 192.168.1.70 metric 100
169.254.0.0/16 dev wlp4s0 scope link metric 1000
192.168.1.0/24 dev wlp4s0 proto kernel scope link src 192.168.1.70 metric 100

# Extract data from example output
Interface (Wifi or Ethernet): wlp4s0
Default Gateway: 192.168.1.254
Network Mask: /24 or 255.255.255.0
Ip range: 192.168.1.0 - 192.168.1.254 (Static ip can take these values)

# Add these lines (WiFi)
wifis:
	<wifi-interface>:
		dhcp4: false
		addresses: [<static-ip>/24]
		gateway4: <default-gateway>
		nameservers:
			addresses: [8.8.8.8,8.8.8.4]
		access-points:
			"<wifi-name>":
				password: "<wifi-password>"
```