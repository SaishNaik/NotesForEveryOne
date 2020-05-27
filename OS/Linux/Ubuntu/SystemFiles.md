# Files in Ubuntu and their significance

### /etc/hosts

A entry for mydomain means that the system will not do a DNS lookup for mydomain, it will be automatically redirected to the IP address you specified in your hosts file. 

### /etc/nsswitch.conf. 
It provides Name Service Switch functionality which controls the order in which services are queried for name service lookups.
Suppose you look for `mydomain.com` and  in `/etc/nsswitch.conf`, it is `hosts:files mdns4_minimal [NOTFOUND=return] dns  myhostname`, that means your host file will be read before going to dns for hostname resolution. 



