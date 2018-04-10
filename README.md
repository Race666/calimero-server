# calimero-server

This script installs the KNXNet/IP Server and tools from the [calimero project](https://calimero-project.github.io/) on a Raspberry Pi or Orange Pi PC

Default configuration is to access the KNX bus by a TPUART Module but 
KNX IP, KNX USB, KNX RF USB and FT1.2 serial access are also possible.

In detail:
- Recognition on which device the script runs
- Setup the serial device depending on the device
- Gets all sources for calimero server and –tools from github
- Complies all sources
- Patches calimero server to run as daemon in background
- Installs binaries to /opt/calimero-server
- Moves/installs config files to /etc/calimero
- Alters config to use a TPUART Module
- Adds 8 Client Addresses
- Sets the Servername
- Creates a user and group knx under which the server runs
- Adds a systemd service knx.service
- Installs calimero tools and a wrapper script knxtools to /usr/local/bin

For more details visit my [blog](https://michlstechblog.info/blog/eib-knx-knxnet-ip-gateway-with-calimero-server-on-raspberry-pi-orange-pi-pc/)


