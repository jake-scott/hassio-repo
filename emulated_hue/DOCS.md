# Emulated Hue for Home Assistant

This is the stable version of the addon. 

## Configuration Options

### Option: `http_port`

Enter an integer to specify a custom http port. This defaults to port 80 if not specified. 

### Option: `https_port`

Enter an integer to specify a custom https port. This defaults to port 443 if not specified.

### Option: `listen_ip`

Enter an IPv4 address to bind the emulated bridge to. The HTTP and HTTPS servers
will only listen on this address, and it is the address advertised to Hue apps
via mDNS and SSDP discovery. If not specified, the address of the interface with
the default route is auto-detected and the servers listen on all interfaces.
Use this if your host has multiple network interfaces (for example VLANs, a VPN
or docker bridge networks) and the wrong address is being advertised.

### Option: `verbose`

Enter true or false to toggle verbose logging. This will provided increase logs for debugging.
