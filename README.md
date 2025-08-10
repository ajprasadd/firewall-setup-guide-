firewall setup and testing in linux operating system

using various commands

sudo ufw status
sudo apt install ufw -y
sudo ufw enable
sudo ufw status numbered
sudo ufw deny 23/tcp
telnet localhost 23
sudo ufw allow 22/tcp
sudo ufw delete <rule_number>

🛡 How Firewall Filters Traffic
UFW is a frontend for iptables.

Rules allow or deny traffic based on port, protocol, and direction.

Default policy: deny incoming, allow outgoing.

Protects against unauthorized access and reduces attack surface.

✅ Conclusion
Successfully blocked Telnet (port 23) traffic.

Allowed SSH (port 22) connections.

Verified using telnet test.

Restored firewall to original state after testing.
