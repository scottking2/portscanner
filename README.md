# portscanner


The pyportscanner is used as a way to scan a host or list of hosts for open ports. The scanner has a few command line switches that allow for different use. 

usage: portscanner.py [-h] [-p PORT] [-n] [-u] TARGET

Port scanner to discover open ports on specified hosts.

positional arguments:
  TARGET                Define the target host/s by comma separated IP
                        addresses

optional arguments:
  -h, --help            show this help message and exit
  -p PORT, --port PORT  specify range of ports. Ex: '1-1025' (default), Ex:
                        '22,23', Ex: '22'
  -n, --noping          Assumes targets are available, and no need to check
                        for ICMP ping. Default checks for response by ICMP
                        ping before scan.
  -u, --udp             run UDP scan of the port range as well. **Warning,
                        this may take a long time.


****Warning****
When the UDP switch is used this will make the program slow. 
