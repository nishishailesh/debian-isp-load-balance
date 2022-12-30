# debian-isp-load-balance
## Use
It is useful if server have two ISP connection at different interfaces and third interface is connected to local LAN (where server distributes internet)\
e.g 
eth0 connected to ISP1\
eth1 connected to ISP2\
eth3 connected to LAN\

## Install Net-ISP-Balance
```git pull https://github.com/lstein/Net-ISP-Balance```\
```perl ./Build.PL```\
It may give error because Module::Build is not installed\
```cpan Module::Build```\
It may give error because  ```make``` is not installed\
```apt install make```\
```cpan Module::Build```\
```perl ./Build.PL```\
a script named "Build" is added in installation folder
```perl Build installdeps```\
```./Build test```\
```./Build install```\
Functioning program require iptables (not nftables)
```apt install iptables```
## setup and running
excecutable is called ```load_balance.pl```\
configuration is stored  in /etc/network/balance.conf\
read instructions and modify balance.conf\
```load_balance.pl```\
## Test functioning of load balance
run following command reapeatedly\
```traceroute google.com```\
Notice how different route is taken everytime\
enjoy

