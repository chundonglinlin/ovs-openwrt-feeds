openvswitch
===========

UPDATE: Works now with OpenWrt "Barrier Breaker" (Bleeding Edge)

Installation
------------

Install this as a feed!

### Installation in OpenWrt

> cd $TOPDIR
> 
> echo 'src-git openvswitch git://github.com/chundonglinlin/ovs-openwrt-feeds.git' >> feeds.conf
>
> ./scripts/feeds update openvswitch
>
> ./scripts/feeds install -a -p openvswitch
> 
> make menuconfig
>
> select Network -> openvswitch-switch, openvswitch-brcompat and openvswitch-controller
>
### Cancel Kernel Bridge
> echo '# CONFIG_KERNEL_BRIDGE is not set' >> .config


Development
-----------

Please fork on github and send pull requests.

