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

###添加一个 patch
> wget https://gist.githubusercontent.com/pichuang/7372af6d5d3bd1db5a88/raw/4e2290e3e184288de7623c02f63fb57c536e035a/openwrt-add-libatomic.patch -q -O - | patch -p1

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

