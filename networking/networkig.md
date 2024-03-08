# Networking
---

## Static Ip address (Ubuntu 20.04+, netplan)

```bash
# Open default netplan config file
sudo nano /etc/netplan/01-network-manager-all.yaml

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