# VPN Connections

VPN Connections allows us to connect to Amazon VPC
There are some options of VPN connections available:
* AWS Site-to-Site VPN: Allows create a IPsec (encrypted connection) between your VPC and your remote network
* AWS Client VPN: Allows you to configure an endpoint to grant the security of the connection of the clients by VPN session with TLS. This allows clients to access AWS or on-premises of anywhere using a VPN client base in OpenVPN.
* AWS VPN CloudHub: If you have more than one remote network (like company branches)you can create many connectins of AWS Site-to_site VPN by using the private virtual gateway, allowing communicatiion between networks.

### References
- [VPN Connections](https://docs.aws.amazon.com/pt_br/vpc/latest/userguide/vpn-connections.html)
