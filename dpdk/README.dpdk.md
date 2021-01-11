
# How to standalone test
 sudo docker run --privileged -it <docker image> bash
snort -Q -v --daq dpdk --daq-dir /usr/local/lib/daq --daq-var debug=1 --daq-var dpdk_args=" -m 256 -c 1 -n4 --no-pci --no-huge --log-level=8 --vdev=eth_af_packet0,iface=eth0" -i eth0:eth0
```


# How to build DPDK deb
from ur linux host
```
./install-dpdk.sh <desired version>
default is 19.11
```

