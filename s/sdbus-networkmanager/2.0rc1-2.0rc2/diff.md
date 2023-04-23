# Comparing `tmp/sdbus-networkmanager-2.0rc1.tar.gz` & `tmp/sdbus-networkmanager-2.0rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sdbus-networkmanager-2.0rc1.tar", last modified: Mon Dec 26 11:16:15 2022, max compression
+gzip compressed data, was "sdbus-networkmanager-2.0rc2.tar", last modified: Sun Apr 23 14:33:57 2023, max compression
```

## Comparing `sdbus-networkmanager-2.0rc1.tar` & `sdbus-networkmanager-2.0rc2.tar`

### file list

```diff
@@ -1,147 +1,149 @@
-drwxr-xr-x   0 igo95862  (1000) igo95862  (1000)        0 2022-12-26 11:16:15.214896 sdbus-networkmanager-2.0rc1/
--rw-r--r--   0 igo95862  (1000) igo95862  (1000)    18092 2021-07-09 19:11:31.000000 sdbus-networkmanager-2.0rc1/COPYING
--rw-r--r--   0 igo95862  (1000) igo95862  (1000)    26530 2021-07-09 19:11:31.000000 sdbus-networkmanager-2.0rc1/COPYING.LESSER
--rw-r--r--   0 igo95862  (1000) igo95862  (1000)     1868 2022-12-26 11:16:15.214896 sdbus-networkmanager-2.0rc1/PKG-INFO
--rw-r--r--   0 igo95862  (1000) igo95862  (1000)      892 2021-07-19 17:24:15.000000 sdbus-networkmanager-2.0rc1/README.md
-drwxr-xr-x   0 igo95862  (1000) igo95862  (1000)        0 2022-12-26 11:16:15.201562 sdbus-networkmanager-2.0rc1/sdbus_async/
-drwxr-xr-x   0 igo95862  (1000) igo95862  (1000)        0 2022-12-26 11:16:15.204895 sdbus-networkmanager-2.0rc1/sdbus_async/networkmanager/
--rw-r--r--   0 igo95862  (1000) igo95862  (1000)    13540 2022-12-24 17:46:17.000000 sdbus-networkmanager-2.0rc1/sdbus_async/networkmanager/__init__.py
--rw-r--r--   0 igo95862  (1000) igo95862  (1000)    14688 2022-07-17 20:31:32.000000 sdbus-networkmanager-2.0rc1/sdbus_async/networkmanager/enums.py
--rw-r--r--   0 igo95862  (1000) igo95862  (1000)    17717 2022-05-28 10:24:43.000000 sdbus-networkmanager-2.0rc1/sdbus_async/networkmanager/exceptions.py
--rw-r--r--   0 igo95862  (1000) igo95862  (1000)    31896 2022-12-26 11:11:35.000000 sdbus-networkmanager-2.0rc1/sdbus_async/networkmanager/interfaces_devices.py
--rw-r--r--   0 igo95862  (1000) igo95862  (1000)    40097 2022-12-26 10:32:55.000000 sdbus-networkmanager-2.0rc1/sdbus_async/networkmanager/interfaces_other.py
--rw-r--r--   0 igo95862  (1000) igo95862  (1000)    36215 2022-07-17 20:31:32.000000 sdbus-networkmanager-2.0rc1/sdbus_async/networkmanager/objects.py
--rw-r--r--   0 igo95862  (1000) igo95862  (1000)        0 2021-07-09 14:39:32.000000 sdbus-networkmanager-2.0rc1/sdbus_async/networkmanager/py.typed
-drwxr-xr-x   0 igo95862  (1000) igo95862  (1000)        0 2022-12-26 11:16:15.208229 sdbus-networkmanager-2.0rc1/sdbus_async/networkmanager/settings/
--rw-r--r--   0 igo95862  (1000) igo95862  (1000)     3587 2022-12-21 19:03:30.000000 sdbus-networkmanager-2.0rc1/sdbus_async/networkmanager/settings/__init__.py
--rw-r--r--   0 igo95862  (1000) igo95862  (1000)     2023 2022-12-21 19:03:30.000000 sdbus-networkmanager-2.0rc1/sdbus_async/networkmanager/settings/adsl.py
--rw-r--r--   0 igo95862  (1000) igo95862  (1000)     4885 2022-12-20 16:56:46.000000 sdbus-networkmanager-2.0rc1/sdbus_async/networkmanager/settings/base.py
--rw-r--r--   0 igo95862  (1000) igo95862  (1000)      955 2022-12-21 19:03:30.000000 sdbus-networkmanager-2.0rc1/sdbus_async/networkmanager/settings/bluetooth.py
--rw-r--r--   0 igo95862  (1000) igo95862  (1000)     1125 2022-12-21 19:03:30.000000 sdbus-networkmanager-2.0rc1/sdbus_async/networkmanager/settings/bond.py
--rw-r--r--   0 igo95862  (1000) igo95862  (1000)      723 2022-12-21 19:03:30.000000 sdbus-networkmanager-2.0rc1/sdbus_async/networkmanager/settings/bond_port.py
--rw-r--r--   0 igo95862  (1000) igo95862  (1000)    10117 2022-12-21 19:03:30.000000 sdbus-networkmanager-2.0rc1/sdbus_async/networkmanager/settings/bridge.py
--rw-r--r--   0 igo95862  (1000) igo95862  (1000)     1952 2022-12-21 19:03:30.000000 sdbus-networkmanager-2.0rc1/sdbus_async/networkmanager/settings/bridge_port.py
--rw-r--r--   0 igo95862  (1000) igo95862  (1000)     2107 2022-12-21 19:03:30.000000 sdbus-networkmanager-2.0rc1/sdbus_async/networkmanager/settings/cdma.py
--rw-r--r--   0 igo95862  (1000) igo95862  (1000)    20276 2022-12-21 19:03:30.000000 sdbus-networkmanager-2.0rc1/sdbus_async/networkmanager/settings/connection.py
--rw-r--r--   0 igo95862  (1000) igo95862  (1000)     7952 2022-12-03 14:35:05.000000 sdbus-networkmanager-2.0rc1/sdbus_async/networkmanager/settings/datatypes.py
--rw-r--r--   0 igo95862  (1000) igo95862  (1000)     6660 2022-12-21 19:03:30.000000 sdbus-networkmanager-2.0rc1/sdbus_async/networkmanager/settings/dcb.py
--rw-r--r--   0 igo95862  (1000) igo95862  (1000)      428 2022-12-21 19:03:30.000000 sdbus-networkmanager-2.0rc1/sdbus_async/networkmanager/settings/dummy.py
--rw-r--r--   0 igo95862  (1000) igo95862  (1000)    25028 2022-12-21 19:03:30.000000 sdbus-networkmanager-2.0rc1/sdbus_async/networkmanager/settings/eapol.py
--rw-r--r--   0 igo95862  (1000) igo95862  (1000)    11472 2022-12-21 19:03:30.000000 sdbus-networkmanager-2.0rc1/sdbus_async/networkmanager/settings/ethernet.py
--rw-r--r--   0 igo95862  (1000) igo95862  (1000)      436 2022-12-21 19:03:30.000000 sdbus-networkmanager-2.0rc1/sdbus_async/networkmanager/settings/ethtool.py
--rw-r--r--   0 igo95862  (1000) igo95862  (1000)      432 2022-12-21 19:03:30.000000 sdbus-networkmanager-2.0rc1/sdbus_async/networkmanager/settings/generic.py
--rw-r--r--   0 igo95862  (1000) igo95862  (1000)     5654 2022-12-21 19:03:30.000000 sdbus-networkmanager-2.0rc1/sdbus_async/networkmanager/settings/gsm.py
--rw-r--r--   0 igo95862  (1000) igo95862  (1000)     3065 2022-12-21 19:03:30.000000 sdbus-networkmanager-2.0rc1/sdbus_async/networkmanager/settings/hostname.py
--rw-r--r--   0 igo95862  (1000) igo95862  (1000)     2118 2022-12-21 19:03:30.000000 sdbus-networkmanager-2.0rc1/sdbus_async/networkmanager/settings/infiniband.py
--rw-r--r--   0 igo95862  (1000) igo95862  (1000)     4404 2022-12-21 19:03:30.000000 sdbus-networkmanager-2.0rc1/sdbus_async/networkmanager/settings/ip_tunnel.py
--rw-r--r--   0 igo95862  (1000) igo95862  (1000)    23497 2022-12-21 19:03:30.000000 sdbus-networkmanager-2.0rc1/sdbus_async/networkmanager/settings/ipv4.py
--rw-r--r--   0 igo95862  (1000) igo95862  (1000)    25961 2022-12-21 19:03:30.000000 sdbus-networkmanager-2.0rc1/sdbus_async/networkmanager/settings/ipv6.py
--rw-r--r--   0 igo95862  (1000) igo95862  (1000)      723 2022-12-21 19:03:30.000000 sdbus-networkmanager-2.0rc1/sdbus_async/networkmanager/settings/lowpan.py
--rw-r--r--   0 igo95862  (1000) igo95862  (1000)     2881 2022-12-21 19:03:30.000000 sdbus-networkmanager-2.0rc1/sdbus_async/networkmanager/settings/macsec.py
--rw-r--r--   0 igo95862  (1000) igo95862  (1000)     1581 2022-12-21 19:03:30.000000 sdbus-networkmanager-2.0rc1/sdbus_async/networkmanager/settings/macvlan.py
--rw-r--r--   0 igo95862  (1000) igo95862  (1000)     3993 2022-12-21 19:03:30.000000 sdbus-networkmanager-2.0rc1/sdbus_async/networkmanager/settings/match.py
--rw-r--r--   0 igo95862  (1000) igo95862  (1000)     1296 2022-12-21 19:03:30.000000 sdbus-networkmanager-2.0rc1/sdbus_async/networkmanager/settings/olpc_mesh.py
--rw-r--r--   0 igo95862  (1000) igo95862  (1000)     1553 2022-12-21 19:03:30.000000 sdbus-networkmanager-2.0rc1/sdbus_async/networkmanager/settings/ovs_bridge.py
--rw-r--r--   0 igo95862  (1000) igo95862  (1000)      960 2022-12-21 19:03:30.000000 sdbus-networkmanager-2.0rc1/sdbus_async/networkmanager/settings/ovs_dpdk.py
--rw-r--r--   0 igo95862  (1000) igo95862  (1000)      686 2022-12-21 19:03:30.000000 sdbus-networkmanager-2.0rc1/sdbus_async/networkmanager/settings/ovs_external_ids.py
--rw-r--r--   0 igo95862  (1000) igo95862  (1000)     1242 2022-12-21 19:03:30.000000 sdbus-networkmanager-2.0rc1/sdbus_async/networkmanager/settings/ovs_interface.py
--rw-r--r--   0 igo95862  (1000) igo95862  (1000)      737 2022-12-21 19:03:30.000000 sdbus-networkmanager-2.0rc1/sdbus_async/networkmanager/settings/ovs_patch.py
--rw-r--r--   0 igo95862  (1000) igo95862  (1000)     1843 2022-12-21 19:03:30.000000 sdbus-networkmanager-2.0rc1/sdbus_async/networkmanager/settings/ovs_port.py
--rw-r--r--   0 igo95862  (1000) igo95862  (1000)     5940 2022-12-21 19:03:30.000000 sdbus-networkmanager-2.0rc1/sdbus_async/networkmanager/settings/ppp.py
--rw-r--r--   0 igo95862  (1000) igo95862  (1000)     2065 2022-12-21 19:03:30.000000 sdbus-networkmanager-2.0rc1/sdbus_async/networkmanager/settings/pppoe.py
--rw-r--r--   0 igo95862  (1000) igo95862  (1000)    17923 2022-12-21 19:03:30.000000 sdbus-networkmanager-2.0rc1/sdbus_async/networkmanager/settings/profile.py
--rw-r--r--   0 igo95862  (1000) igo95862  (1000)     1406 2022-12-21 19:03:30.000000 sdbus-networkmanager-2.0rc1/sdbus_async/networkmanager/settings/proxy.py
--rw-r--r--   0 igo95862  (1000) igo95862  (1000)     1761 2022-12-21 19:03:30.000000 sdbus-networkmanager-2.0rc1/sdbus_async/networkmanager/settings/serial.py
--rw-r--r--   0 igo95862  (1000) igo95862  (1000)     2667 2022-12-21 19:03:30.000000 sdbus-networkmanager-2.0rc1/sdbus_async/networkmanager/settings/sriov.py
--rw-r--r--   0 igo95862  (1000) igo95862  (1000)     1673 2022-12-21 19:03:30.000000 sdbus-networkmanager-2.0rc1/sdbus_async/networkmanager/settings/tc.py
--rw-r--r--   0 igo95862  (1000) igo95862  (1000)     5537 2022-12-21 19:03:30.000000 sdbus-networkmanager-2.0rc1/sdbus_async/networkmanager/settings/team.py
--rw-r--r--   0 igo95862  (1000) igo95862  (1000)     2935 2022-12-21 19:03:30.000000 sdbus-networkmanager-2.0rc1/sdbus_async/networkmanager/settings/team_port.py
--rw-r--r--   0 igo95862  (1000) igo95862  (1000)     2222 2022-12-21 19:03:30.000000 sdbus-networkmanager-2.0rc1/sdbus_async/networkmanager/settings/tun.py
--rw-r--r--   0 igo95862  (1000) igo95862  (1000)      876 2022-12-21 19:03:30.000000 sdbus-networkmanager-2.0rc1/sdbus_async/networkmanager/settings/user.py
--rw-r--r--   0 igo95862  (1000) igo95862  (1000)      678 2022-12-21 19:03:30.000000 sdbus-networkmanager-2.0rc1/sdbus_async/networkmanager/settings/veth.py
--rw-r--r--   0 igo95862  (1000) igo95862  (1000)     3148 2022-12-21 19:03:30.000000 sdbus-networkmanager-2.0rc1/sdbus_async/networkmanager/settings/vlan.py
--rw-r--r--   0 igo95862  (1000) igo95862  (1000)     2749 2022-12-21 19:03:30.000000 sdbus-networkmanager-2.0rc1/sdbus_async/networkmanager/settings/vpn.py
--rw-r--r--   0 igo95862  (1000) igo95862  (1000)      617 2022-12-21 19:03:30.000000 sdbus-networkmanager-2.0rc1/sdbus_async/networkmanager/settings/vrf.py
--rw-r--r--   0 igo95862  (1000) igo95862  (1000)     4529 2022-12-21 19:03:30.000000 sdbus-networkmanager-2.0rc1/sdbus_async/networkmanager/settings/vxlan.py
--rw-r--r--   0 igo95862  (1000) igo95862  (1000)     1550 2022-12-21 19:03:30.000000 sdbus-networkmanager-2.0rc1/sdbus_async/networkmanager/settings/wifi_p2p.py
--rw-r--r--   0 igo95862  (1000) igo95862  (1000)     1059 2022-12-21 19:03:30.000000 sdbus-networkmanager-2.0rc1/sdbus_async/networkmanager/settings/wimax.py
--rw-r--r--   0 igo95862  (1000) igo95862  (1000)     4838 2022-12-21 19:03:30.000000 sdbus-networkmanager-2.0rc1/sdbus_async/networkmanager/settings/wireguard.py
--rw-r--r--   0 igo95862  (1000) igo95862  (1000)    12562 2022-12-21 19:03:30.000000 sdbus-networkmanager-2.0rc1/sdbus_async/networkmanager/settings/wireless.py
--rw-r--r--   0 igo95862  (1000) igo95862  (1000)     9087 2022-12-21 19:03:30.000000 sdbus-networkmanager-2.0rc1/sdbus_async/networkmanager/settings/wireless_security.py
--rw-r--r--   0 igo95862  (1000) igo95862  (1000)     1802 2022-12-21 19:03:30.000000 sdbus-networkmanager-2.0rc1/sdbus_async/networkmanager/settings/wpan.py
--rw-r--r--   0 igo95862  (1000) igo95862  (1000)     1441 2022-05-28 17:36:59.000000 sdbus-networkmanager-2.0rc1/sdbus_async/networkmanager/types.py
-drwxr-xr-x   0 igo95862  (1000) igo95862  (1000)        0 2022-12-26 11:16:15.201562 sdbus-networkmanager-2.0rc1/sdbus_block/
-drwxr-xr-x   0 igo95862  (1000) igo95862  (1000)        0 2022-12-26 11:16:15.208229 sdbus-networkmanager-2.0rc1/sdbus_block/networkmanager/
--rw-r--r--   0 igo95862  (1000) igo95862  (1000)    13130 2022-11-14 18:24:48.000000 sdbus-networkmanager-2.0rc1/sdbus_block/networkmanager/__init__.py
--rw-r--r--   0 igo95862  (1000) igo95862  (1000)    14688 2022-07-17 20:31:32.000000 sdbus-networkmanager-2.0rc1/sdbus_block/networkmanager/enums.py
--rw-r--r--   0 igo95862  (1000) igo95862  (1000)    17717 2022-05-28 10:24:43.000000 sdbus-networkmanager-2.0rc1/sdbus_block/networkmanager/exceptions.py
--rw-r--r--   0 igo95862  (1000) igo95862  (1000)    29700 2022-12-26 11:11:21.000000 sdbus-networkmanager-2.0rc1/sdbus_block/networkmanager/interfaces_devices.py
--rw-r--r--   0 igo95862  (1000) igo95862  (1000)    35524 2022-12-26 10:32:48.000000 sdbus-networkmanager-2.0rc1/sdbus_block/networkmanager/interfaces_other.py
--rw-r--r--   0 igo95862  (1000) igo95862  (1000)    33988 2022-07-17 20:31:32.000000 sdbus-networkmanager-2.0rc1/sdbus_block/networkmanager/objects.py
--rw-r--r--   0 igo95862  (1000) igo95862  (1000)        0 2021-07-09 14:39:32.000000 sdbus-networkmanager-2.0rc1/sdbus_block/networkmanager/py.typed
-drwxr-xr-x   0 igo95862  (1000) igo95862  (1000)        0 2022-12-26 11:16:15.214896 sdbus-networkmanager-2.0rc1/sdbus_block/networkmanager/settings/
--rw-r--r--   0 igo95862  (1000) igo95862  (1000)     3587 2022-12-21 19:03:30.000000 sdbus-networkmanager-2.0rc1/sdbus_block/networkmanager/settings/__init__.py
--rw-r--r--   0 igo95862  (1000) igo95862  (1000)     2023 2022-12-21 19:03:30.000000 sdbus-networkmanager-2.0rc1/sdbus_block/networkmanager/settings/adsl.py
--rw-r--r--   0 igo95862  (1000) igo95862  (1000)     4885 2022-12-20 16:56:46.000000 sdbus-networkmanager-2.0rc1/sdbus_block/networkmanager/settings/base.py
--rw-r--r--   0 igo95862  (1000) igo95862  (1000)      955 2022-12-21 19:03:30.000000 sdbus-networkmanager-2.0rc1/sdbus_block/networkmanager/settings/bluetooth.py
--rw-r--r--   0 igo95862  (1000) igo95862  (1000)     1125 2022-12-21 19:03:30.000000 sdbus-networkmanager-2.0rc1/sdbus_block/networkmanager/settings/bond.py
--rw-r--r--   0 igo95862  (1000) igo95862  (1000)      723 2022-12-21 19:03:30.000000 sdbus-networkmanager-2.0rc1/sdbus_block/networkmanager/settings/bond_port.py
--rw-r--r--   0 igo95862  (1000) igo95862  (1000)    10117 2022-12-21 19:03:30.000000 sdbus-networkmanager-2.0rc1/sdbus_block/networkmanager/settings/bridge.py
--rw-r--r--   0 igo95862  (1000) igo95862  (1000)     1952 2022-12-21 19:03:30.000000 sdbus-networkmanager-2.0rc1/sdbus_block/networkmanager/settings/bridge_port.py
--rw-r--r--   0 igo95862  (1000) igo95862  (1000)     2107 2022-12-21 19:03:30.000000 sdbus-networkmanager-2.0rc1/sdbus_block/networkmanager/settings/cdma.py
--rw-r--r--   0 igo95862  (1000) igo95862  (1000)    20276 2022-12-21 19:03:30.000000 sdbus-networkmanager-2.0rc1/sdbus_block/networkmanager/settings/connection.py
--rw-r--r--   0 igo95862  (1000) igo95862  (1000)     7952 2022-12-03 14:35:05.000000 sdbus-networkmanager-2.0rc1/sdbus_block/networkmanager/settings/datatypes.py
--rw-r--r--   0 igo95862  (1000) igo95862  (1000)     6660 2022-12-21 19:03:30.000000 sdbus-networkmanager-2.0rc1/sdbus_block/networkmanager/settings/dcb.py
--rw-r--r--   0 igo95862  (1000) igo95862  (1000)      428 2022-12-21 19:03:30.000000 sdbus-networkmanager-2.0rc1/sdbus_block/networkmanager/settings/dummy.py
--rw-r--r--   0 igo95862  (1000) igo95862  (1000)    25028 2022-12-21 19:03:30.000000 sdbus-networkmanager-2.0rc1/sdbus_block/networkmanager/settings/eapol.py
--rw-r--r--   0 igo95862  (1000) igo95862  (1000)    11472 2022-12-21 19:03:30.000000 sdbus-networkmanager-2.0rc1/sdbus_block/networkmanager/settings/ethernet.py
--rw-r--r--   0 igo95862  (1000) igo95862  (1000)      436 2022-12-21 19:03:30.000000 sdbus-networkmanager-2.0rc1/sdbus_block/networkmanager/settings/ethtool.py
--rw-r--r--   0 igo95862  (1000) igo95862  (1000)      432 2022-12-21 19:03:30.000000 sdbus-networkmanager-2.0rc1/sdbus_block/networkmanager/settings/generic.py
--rw-r--r--   0 igo95862  (1000) igo95862  (1000)     5654 2022-12-21 19:03:30.000000 sdbus-networkmanager-2.0rc1/sdbus_block/networkmanager/settings/gsm.py
--rw-r--r--   0 igo95862  (1000) igo95862  (1000)     3065 2022-12-21 19:03:30.000000 sdbus-networkmanager-2.0rc1/sdbus_block/networkmanager/settings/hostname.py
--rw-r--r--   0 igo95862  (1000) igo95862  (1000)     2118 2022-12-21 19:03:30.000000 sdbus-networkmanager-2.0rc1/sdbus_block/networkmanager/settings/infiniband.py
--rw-r--r--   0 igo95862  (1000) igo95862  (1000)     4404 2022-12-21 19:03:30.000000 sdbus-networkmanager-2.0rc1/sdbus_block/networkmanager/settings/ip_tunnel.py
--rw-r--r--   0 igo95862  (1000) igo95862  (1000)    23497 2022-12-21 19:03:30.000000 sdbus-networkmanager-2.0rc1/sdbus_block/networkmanager/settings/ipv4.py
--rw-r--r--   0 igo95862  (1000) igo95862  (1000)    25961 2022-12-21 19:03:30.000000 sdbus-networkmanager-2.0rc1/sdbus_block/networkmanager/settings/ipv6.py
--rw-r--r--   0 igo95862  (1000) igo95862  (1000)      723 2022-12-21 19:03:30.000000 sdbus-networkmanager-2.0rc1/sdbus_block/networkmanager/settings/lowpan.py
--rw-r--r--   0 igo95862  (1000) igo95862  (1000)     2881 2022-12-21 19:03:30.000000 sdbus-networkmanager-2.0rc1/sdbus_block/networkmanager/settings/macsec.py
--rw-r--r--   0 igo95862  (1000) igo95862  (1000)     1581 2022-12-21 19:03:30.000000 sdbus-networkmanager-2.0rc1/sdbus_block/networkmanager/settings/macvlan.py
--rw-r--r--   0 igo95862  (1000) igo95862  (1000)     3993 2022-12-21 19:03:30.000000 sdbus-networkmanager-2.0rc1/sdbus_block/networkmanager/settings/match.py
--rw-r--r--   0 igo95862  (1000) igo95862  (1000)     1296 2022-12-21 19:03:30.000000 sdbus-networkmanager-2.0rc1/sdbus_block/networkmanager/settings/olpc_mesh.py
--rw-r--r--   0 igo95862  (1000) igo95862  (1000)     1553 2022-12-21 19:03:30.000000 sdbus-networkmanager-2.0rc1/sdbus_block/networkmanager/settings/ovs_bridge.py
--rw-r--r--   0 igo95862  (1000) igo95862  (1000)      960 2022-12-21 19:03:30.000000 sdbus-networkmanager-2.0rc1/sdbus_block/networkmanager/settings/ovs_dpdk.py
--rw-r--r--   0 igo95862  (1000) igo95862  (1000)      686 2022-12-21 19:03:30.000000 sdbus-networkmanager-2.0rc1/sdbus_block/networkmanager/settings/ovs_external_ids.py
--rw-r--r--   0 igo95862  (1000) igo95862  (1000)     1242 2022-12-21 19:03:30.000000 sdbus-networkmanager-2.0rc1/sdbus_block/networkmanager/settings/ovs_interface.py
--rw-r--r--   0 igo95862  (1000) igo95862  (1000)      737 2022-12-21 19:03:30.000000 sdbus-networkmanager-2.0rc1/sdbus_block/networkmanager/settings/ovs_patch.py
--rw-r--r--   0 igo95862  (1000) igo95862  (1000)     1843 2022-12-21 19:03:30.000000 sdbus-networkmanager-2.0rc1/sdbus_block/networkmanager/settings/ovs_port.py
--rw-r--r--   0 igo95862  (1000) igo95862  (1000)     5940 2022-12-21 19:03:30.000000 sdbus-networkmanager-2.0rc1/sdbus_block/networkmanager/settings/ppp.py
--rw-r--r--   0 igo95862  (1000) igo95862  (1000)     2065 2022-12-21 19:03:30.000000 sdbus-networkmanager-2.0rc1/sdbus_block/networkmanager/settings/pppoe.py
--rw-r--r--   0 igo95862  (1000) igo95862  (1000)    17923 2022-12-21 19:03:30.000000 sdbus-networkmanager-2.0rc1/sdbus_block/networkmanager/settings/profile.py
--rw-r--r--   0 igo95862  (1000) igo95862  (1000)     1406 2022-12-21 19:03:30.000000 sdbus-networkmanager-2.0rc1/sdbus_block/networkmanager/settings/proxy.py
--rw-r--r--   0 igo95862  (1000) igo95862  (1000)     1761 2022-12-21 19:03:30.000000 sdbus-networkmanager-2.0rc1/sdbus_block/networkmanager/settings/serial.py
--rw-r--r--   0 igo95862  (1000) igo95862  (1000)     2667 2022-12-21 19:03:30.000000 sdbus-networkmanager-2.0rc1/sdbus_block/networkmanager/settings/sriov.py
--rw-r--r--   0 igo95862  (1000) igo95862  (1000)     1673 2022-12-21 19:03:30.000000 sdbus-networkmanager-2.0rc1/sdbus_block/networkmanager/settings/tc.py
--rw-r--r--   0 igo95862  (1000) igo95862  (1000)     5537 2022-12-21 19:03:30.000000 sdbus-networkmanager-2.0rc1/sdbus_block/networkmanager/settings/team.py
--rw-r--r--   0 igo95862  (1000) igo95862  (1000)     2935 2022-12-21 19:03:30.000000 sdbus-networkmanager-2.0rc1/sdbus_block/networkmanager/settings/team_port.py
--rw-r--r--   0 igo95862  (1000) igo95862  (1000)     2222 2022-12-21 19:03:30.000000 sdbus-networkmanager-2.0rc1/sdbus_block/networkmanager/settings/tun.py
--rw-r--r--   0 igo95862  (1000) igo95862  (1000)      876 2022-12-21 19:03:30.000000 sdbus-networkmanager-2.0rc1/sdbus_block/networkmanager/settings/user.py
--rw-r--r--   0 igo95862  (1000) igo95862  (1000)      678 2022-12-21 19:03:30.000000 sdbus-networkmanager-2.0rc1/sdbus_block/networkmanager/settings/veth.py
--rw-r--r--   0 igo95862  (1000) igo95862  (1000)     3148 2022-12-21 19:03:30.000000 sdbus-networkmanager-2.0rc1/sdbus_block/networkmanager/settings/vlan.py
--rw-r--r--   0 igo95862  (1000) igo95862  (1000)     2749 2022-12-21 19:03:30.000000 sdbus-networkmanager-2.0rc1/sdbus_block/networkmanager/settings/vpn.py
--rw-r--r--   0 igo95862  (1000) igo95862  (1000)      617 2022-12-21 19:03:30.000000 sdbus-networkmanager-2.0rc1/sdbus_block/networkmanager/settings/vrf.py
--rw-r--r--   0 igo95862  (1000) igo95862  (1000)     4529 2022-12-21 19:03:30.000000 sdbus-networkmanager-2.0rc1/sdbus_block/networkmanager/settings/vxlan.py
--rw-r--r--   0 igo95862  (1000) igo95862  (1000)     1550 2022-12-21 19:03:30.000000 sdbus-networkmanager-2.0rc1/sdbus_block/networkmanager/settings/wifi_p2p.py
--rw-r--r--   0 igo95862  (1000) igo95862  (1000)     1059 2022-12-21 19:03:30.000000 sdbus-networkmanager-2.0rc1/sdbus_block/networkmanager/settings/wimax.py
--rw-r--r--   0 igo95862  (1000) igo95862  (1000)     4838 2022-12-21 19:03:30.000000 sdbus-networkmanager-2.0rc1/sdbus_block/networkmanager/settings/wireguard.py
--rw-r--r--   0 igo95862  (1000) igo95862  (1000)    12562 2022-12-21 19:03:30.000000 sdbus-networkmanager-2.0rc1/sdbus_block/networkmanager/settings/wireless.py
--rw-r--r--   0 igo95862  (1000) igo95862  (1000)     9087 2022-12-21 19:03:30.000000 sdbus-networkmanager-2.0rc1/sdbus_block/networkmanager/settings/wireless_security.py
--rw-r--r--   0 igo95862  (1000) igo95862  (1000)     1802 2022-12-21 19:03:30.000000 sdbus-networkmanager-2.0rc1/sdbus_block/networkmanager/settings/wpan.py
--rw-r--r--   0 igo95862  (1000) igo95862  (1000)     1441 2022-05-28 17:36:59.000000 sdbus-networkmanager-2.0rc1/sdbus_block/networkmanager/types.py
-drwxr-xr-x   0 igo95862  (1000) igo95862  (1000)        0 2022-12-26 11:16:15.214896 sdbus-networkmanager-2.0rc1/sdbus_networkmanager.egg-info/
--rw-r--r--   0 igo95862  (1000) igo95862  (1000)     1868 2022-12-26 11:16:15.000000 sdbus-networkmanager-2.0rc1/sdbus_networkmanager.egg-info/PKG-INFO
--rw-r--r--   0 igo95862  (1000) igo95862  (1000)     6126 2022-12-26 11:16:15.000000 sdbus-networkmanager-2.0rc1/sdbus_networkmanager.egg-info/SOURCES.txt
--rw-r--r--   0 igo95862  (1000) igo95862  (1000)        1 2022-12-26 11:16:15.000000 sdbus-networkmanager-2.0rc1/sdbus_networkmanager.egg-info/dependency_links.txt
--rw-r--r--   0 igo95862  (1000) igo95862  (1000)       14 2022-12-26 11:16:15.000000 sdbus-networkmanager-2.0rc1/sdbus_networkmanager.egg-info/requires.txt
--rw-r--r--   0 igo95862  (1000) igo95862  (1000)       24 2022-12-26 11:16:15.000000 sdbus-networkmanager-2.0rc1/sdbus_networkmanager.egg-info/top_level.txt
--rw-r--r--   0 igo95862  (1000) igo95862  (1000)       38 2022-12-26 11:16:15.214896 sdbus-networkmanager-2.0rc1/setup.cfg
--rw-r--r--   0 igo95862  (1000) igo95862  (1000)     2516 2022-12-26 11:15:55.000000 sdbus-networkmanager-2.0rc1/setup.py
+drwxr-xr-x   0 igo95862  (1000) igo95862  (1000)        0 2023-04-23 14:33:57.167688 sdbus-networkmanager-2.0rc2/
+-rw-r--r--   0 igo95862  (1000) igo95862  (1000)    18092 2021-07-09 19:11:31.000000 sdbus-networkmanager-2.0rc2/COPYING
+-rw-r--r--   0 igo95862  (1000) igo95862  (1000)    26530 2021-07-09 19:11:31.000000 sdbus-networkmanager-2.0rc2/COPYING.LESSER
+-rw-r--r--   0 igo95862  (1000) igo95862  (1000)     1868 2023-04-23 14:33:57.167688 sdbus-networkmanager-2.0rc2/PKG-INFO
+-rw-r--r--   0 igo95862  (1000) igo95862  (1000)      892 2021-07-19 17:24:15.000000 sdbus-networkmanager-2.0rc2/README.md
+drwxr-xr-x   0 igo95862  (1000) igo95862  (1000)        0 2023-04-23 14:33:57.147688 sdbus-networkmanager-2.0rc2/sdbus_async/
+drwxr-xr-x   0 igo95862  (1000) igo95862  (1000)        0 2023-04-23 14:33:57.151021 sdbus-networkmanager-2.0rc2/sdbus_async/networkmanager/
+-rw-r--r--   0 igo95862  (1000) igo95862  (1000)    13540 2022-12-24 17:46:17.000000 sdbus-networkmanager-2.0rc2/sdbus_async/networkmanager/__init__.py
+-rw-r--r--   0 igo95862  (1000) igo95862  (1000)    14688 2022-07-17 20:31:32.000000 sdbus-networkmanager-2.0rc2/sdbus_async/networkmanager/enums.py
+-rw-r--r--   0 igo95862  (1000) igo95862  (1000)    17717 2022-05-28 10:24:43.000000 sdbus-networkmanager-2.0rc2/sdbus_async/networkmanager/exceptions.py
+-rw-r--r--   0 igo95862  (1000) igo95862  (1000)    31896 2022-12-26 11:11:35.000000 sdbus-networkmanager-2.0rc2/sdbus_async/networkmanager/interfaces_devices.py
+-rw-r--r--   0 igo95862  (1000) igo95862  (1000)    40097 2022-12-26 10:32:55.000000 sdbus-networkmanager-2.0rc2/sdbus_async/networkmanager/interfaces_other.py
+-rw-r--r--   0 igo95862  (1000) igo95862  (1000)    36215 2022-07-17 20:31:32.000000 sdbus-networkmanager-2.0rc2/sdbus_async/networkmanager/objects.py
+-rw-r--r--   0 igo95862  (1000) igo95862  (1000)        0 2021-07-09 14:39:32.000000 sdbus-networkmanager-2.0rc2/sdbus_async/networkmanager/py.typed
+drwxr-xr-x   0 igo95862  (1000) igo95862  (1000)        0 2023-04-23 14:33:57.157688 sdbus-networkmanager-2.0rc2/sdbus_async/networkmanager/settings/
+-rw-r--r--   0 igo95862  (1000) igo95862  (1000)     3587 2023-02-04 08:24:37.000000 sdbus-networkmanager-2.0rc2/sdbus_async/networkmanager/settings/__init__.py
+-rw-r--r--   0 igo95862  (1000) igo95862  (1000)     2023 2023-02-04 08:24:37.000000 sdbus-networkmanager-2.0rc2/sdbus_async/networkmanager/settings/adsl.py
+-rw-r--r--   0 igo95862  (1000) igo95862  (1000)     5012 2023-02-04 09:10:58.000000 sdbus-networkmanager-2.0rc2/sdbus_async/networkmanager/settings/base.py
+-rw-r--r--   0 igo95862  (1000) igo95862  (1000)      955 2023-02-04 08:24:37.000000 sdbus-networkmanager-2.0rc2/sdbus_async/networkmanager/settings/bluetooth.py
+-rw-r--r--   0 igo95862  (1000) igo95862  (1000)     1125 2023-02-04 08:24:37.000000 sdbus-networkmanager-2.0rc2/sdbus_async/networkmanager/settings/bond.py
+-rw-r--r--   0 igo95862  (1000) igo95862  (1000)      723 2023-02-04 08:24:37.000000 sdbus-networkmanager-2.0rc2/sdbus_async/networkmanager/settings/bond_port.py
+-rw-r--r--   0 igo95862  (1000) igo95862  (1000)    10117 2023-02-04 08:24:37.000000 sdbus-networkmanager-2.0rc2/sdbus_async/networkmanager/settings/bridge.py
+-rw-r--r--   0 igo95862  (1000) igo95862  (1000)     1952 2023-02-04 08:24:37.000000 sdbus-networkmanager-2.0rc2/sdbus_async/networkmanager/settings/bridge_port.py
+-rw-r--r--   0 igo95862  (1000) igo95862  (1000)     2107 2023-02-04 08:24:37.000000 sdbus-networkmanager-2.0rc2/sdbus_async/networkmanager/settings/cdma.py
+-rw-r--r--   0 igo95862  (1000) igo95862  (1000)    20276 2023-02-04 08:24:37.000000 sdbus-networkmanager-2.0rc2/sdbus_async/networkmanager/settings/connection.py
+-rw-r--r--   0 igo95862  (1000) igo95862  (1000)     7952 2022-12-03 14:35:05.000000 sdbus-networkmanager-2.0rc2/sdbus_async/networkmanager/settings/datatypes.py
+-rw-r--r--   0 igo95862  (1000) igo95862  (1000)     6660 2023-02-04 08:24:37.000000 sdbus-networkmanager-2.0rc2/sdbus_async/networkmanager/settings/dcb.py
+-rw-r--r--   0 igo95862  (1000) igo95862  (1000)      428 2023-02-04 08:24:37.000000 sdbus-networkmanager-2.0rc2/sdbus_async/networkmanager/settings/dummy.py
+-rw-r--r--   0 igo95862  (1000) igo95862  (1000)    25028 2023-02-04 08:24:37.000000 sdbus-networkmanager-2.0rc2/sdbus_async/networkmanager/settings/eapol.py
+-rw-r--r--   0 igo95862  (1000) igo95862  (1000)    11472 2023-02-04 08:24:37.000000 sdbus-networkmanager-2.0rc2/sdbus_async/networkmanager/settings/ethernet.py
+-rw-r--r--   0 igo95862  (1000) igo95862  (1000)      436 2023-02-04 08:24:37.000000 sdbus-networkmanager-2.0rc2/sdbus_async/networkmanager/settings/ethtool.py
+-rw-r--r--   0 igo95862  (1000) igo95862  (1000)      432 2023-02-04 08:24:37.000000 sdbus-networkmanager-2.0rc2/sdbus_async/networkmanager/settings/generic.py
+-rw-r--r--   0 igo95862  (1000) igo95862  (1000)     5654 2023-02-04 08:24:37.000000 sdbus-networkmanager-2.0rc2/sdbus_async/networkmanager/settings/gsm.py
+-rw-r--r--   0 igo95862  (1000) igo95862  (1000)     3065 2023-02-04 08:24:37.000000 sdbus-networkmanager-2.0rc2/sdbus_async/networkmanager/settings/hostname.py
+-rw-r--r--   0 igo95862  (1000) igo95862  (1000)     2118 2023-02-04 08:24:37.000000 sdbus-networkmanager-2.0rc2/sdbus_async/networkmanager/settings/infiniband.py
+-rw-r--r--   0 igo95862  (1000) igo95862  (1000)     4404 2023-02-04 08:24:37.000000 sdbus-networkmanager-2.0rc2/sdbus_async/networkmanager/settings/ip_tunnel.py
+-rw-r--r--   0 igo95862  (1000) igo95862  (1000)    23497 2023-02-04 08:24:37.000000 sdbus-networkmanager-2.0rc2/sdbus_async/networkmanager/settings/ipv4.py
+-rw-r--r--   0 igo95862  (1000) igo95862  (1000)    25961 2023-02-04 08:24:37.000000 sdbus-networkmanager-2.0rc2/sdbus_async/networkmanager/settings/ipv6.py
+-rw-r--r--   0 igo95862  (1000) igo95862  (1000)      723 2023-02-04 08:24:37.000000 sdbus-networkmanager-2.0rc2/sdbus_async/networkmanager/settings/lowpan.py
+-rw-r--r--   0 igo95862  (1000) igo95862  (1000)     2881 2023-02-04 08:24:37.000000 sdbus-networkmanager-2.0rc2/sdbus_async/networkmanager/settings/macsec.py
+-rw-r--r--   0 igo95862  (1000) igo95862  (1000)     1581 2023-02-04 08:24:37.000000 sdbus-networkmanager-2.0rc2/sdbus_async/networkmanager/settings/macvlan.py
+-rw-r--r--   0 igo95862  (1000) igo95862  (1000)     3993 2023-02-04 08:24:37.000000 sdbus-networkmanager-2.0rc2/sdbus_async/networkmanager/settings/match.py
+-rw-r--r--   0 igo95862  (1000) igo95862  (1000)     1296 2023-02-04 08:24:37.000000 sdbus-networkmanager-2.0rc2/sdbus_async/networkmanager/settings/olpc_mesh.py
+-rw-r--r--   0 igo95862  (1000) igo95862  (1000)     1553 2023-02-04 08:24:37.000000 sdbus-networkmanager-2.0rc2/sdbus_async/networkmanager/settings/ovs_bridge.py
+-rw-r--r--   0 igo95862  (1000) igo95862  (1000)      960 2023-02-04 08:24:37.000000 sdbus-networkmanager-2.0rc2/sdbus_async/networkmanager/settings/ovs_dpdk.py
+-rw-r--r--   0 igo95862  (1000) igo95862  (1000)      686 2023-02-04 08:24:37.000000 sdbus-networkmanager-2.0rc2/sdbus_async/networkmanager/settings/ovs_external_ids.py
+-rw-r--r--   0 igo95862  (1000) igo95862  (1000)     1242 2023-02-04 08:24:37.000000 sdbus-networkmanager-2.0rc2/sdbus_async/networkmanager/settings/ovs_interface.py
+-rw-r--r--   0 igo95862  (1000) igo95862  (1000)      737 2023-02-04 08:24:37.000000 sdbus-networkmanager-2.0rc2/sdbus_async/networkmanager/settings/ovs_patch.py
+-rw-r--r--   0 igo95862  (1000) igo95862  (1000)     1843 2023-02-04 08:24:37.000000 sdbus-networkmanager-2.0rc2/sdbus_async/networkmanager/settings/ovs_port.py
+-rw-r--r--   0 igo95862  (1000) igo95862  (1000)     5940 2023-02-04 08:24:37.000000 sdbus-networkmanager-2.0rc2/sdbus_async/networkmanager/settings/ppp.py
+-rw-r--r--   0 igo95862  (1000) igo95862  (1000)     2065 2023-02-04 08:24:37.000000 sdbus-networkmanager-2.0rc2/sdbus_async/networkmanager/settings/pppoe.py
+-rw-r--r--   0 igo95862  (1000) igo95862  (1000)    17923 2023-02-04 08:24:37.000000 sdbus-networkmanager-2.0rc2/sdbus_async/networkmanager/settings/profile.py
+-rw-r--r--   0 igo95862  (1000) igo95862  (1000)     1406 2023-02-04 08:24:37.000000 sdbus-networkmanager-2.0rc2/sdbus_async/networkmanager/settings/proxy.py
+-rw-r--r--   0 igo95862  (1000) igo95862  (1000)     1761 2023-02-04 08:24:37.000000 sdbus-networkmanager-2.0rc2/sdbus_async/networkmanager/settings/serial.py
+-rw-r--r--   0 igo95862  (1000) igo95862  (1000)     2667 2023-02-04 08:24:37.000000 sdbus-networkmanager-2.0rc2/sdbus_async/networkmanager/settings/sriov.py
+-rw-r--r--   0 igo95862  (1000) igo95862  (1000)     1673 2023-02-04 08:24:37.000000 sdbus-networkmanager-2.0rc2/sdbus_async/networkmanager/settings/tc.py
+-rw-r--r--   0 igo95862  (1000) igo95862  (1000)     5537 2023-02-04 08:24:37.000000 sdbus-networkmanager-2.0rc2/sdbus_async/networkmanager/settings/team.py
+-rw-r--r--   0 igo95862  (1000) igo95862  (1000)     2935 2023-02-04 08:24:37.000000 sdbus-networkmanager-2.0rc2/sdbus_async/networkmanager/settings/team_port.py
+-rw-r--r--   0 igo95862  (1000) igo95862  (1000)     2222 2023-02-04 08:24:37.000000 sdbus-networkmanager-2.0rc2/sdbus_async/networkmanager/settings/tun.py
+-rw-r--r--   0 igo95862  (1000) igo95862  (1000)      876 2023-02-04 08:24:37.000000 sdbus-networkmanager-2.0rc2/sdbus_async/networkmanager/settings/user.py
+-rw-r--r--   0 igo95862  (1000) igo95862  (1000)      678 2023-02-04 08:24:37.000000 sdbus-networkmanager-2.0rc2/sdbus_async/networkmanager/settings/veth.py
+-rw-r--r--   0 igo95862  (1000) igo95862  (1000)     3148 2023-02-04 08:24:37.000000 sdbus-networkmanager-2.0rc2/sdbus_async/networkmanager/settings/vlan.py
+-rw-r--r--   0 igo95862  (1000) igo95862  (1000)     2749 2023-02-04 08:24:37.000000 sdbus-networkmanager-2.0rc2/sdbus_async/networkmanager/settings/vpn.py
+-rw-r--r--   0 igo95862  (1000) igo95862  (1000)      617 2023-02-04 08:24:37.000000 sdbus-networkmanager-2.0rc2/sdbus_async/networkmanager/settings/vrf.py
+-rw-r--r--   0 igo95862  (1000) igo95862  (1000)     4529 2023-02-04 08:24:37.000000 sdbus-networkmanager-2.0rc2/sdbus_async/networkmanager/settings/vxlan.py
+-rw-r--r--   0 igo95862  (1000) igo95862  (1000)     1550 2023-02-04 08:24:37.000000 sdbus-networkmanager-2.0rc2/sdbus_async/networkmanager/settings/wifi_p2p.py
+-rw-r--r--   0 igo95862  (1000) igo95862  (1000)     1059 2023-02-04 08:24:37.000000 sdbus-networkmanager-2.0rc2/sdbus_async/networkmanager/settings/wimax.py
+-rw-r--r--   0 igo95862  (1000) igo95862  (1000)     4838 2023-02-04 08:24:37.000000 sdbus-networkmanager-2.0rc2/sdbus_async/networkmanager/settings/wireguard.py
+-rw-r--r--   0 igo95862  (1000) igo95862  (1000)    12562 2023-02-04 08:24:37.000000 sdbus-networkmanager-2.0rc2/sdbus_async/networkmanager/settings/wireless.py
+-rw-r--r--   0 igo95862  (1000) igo95862  (1000)     9087 2023-02-04 08:24:37.000000 sdbus-networkmanager-2.0rc2/sdbus_async/networkmanager/settings/wireless_security.py
+-rw-r--r--   0 igo95862  (1000) igo95862  (1000)     1802 2023-02-04 08:24:37.000000 sdbus-networkmanager-2.0rc2/sdbus_async/networkmanager/settings/wpan.py
+-rw-r--r--   0 igo95862  (1000) igo95862  (1000)     1441 2022-05-28 17:36:59.000000 sdbus-networkmanager-2.0rc2/sdbus_async/networkmanager/types.py
+drwxr-xr-x   0 igo95862  (1000) igo95862  (1000)        0 2023-04-23 14:33:57.147688 sdbus-networkmanager-2.0rc2/sdbus_block/
+drwxr-xr-x   0 igo95862  (1000) igo95862  (1000)        0 2023-04-23 14:33:57.161021 sdbus-networkmanager-2.0rc2/sdbus_block/networkmanager/
+-rw-r--r--   0 igo95862  (1000) igo95862  (1000)    13130 2022-11-14 18:24:48.000000 sdbus-networkmanager-2.0rc2/sdbus_block/networkmanager/__init__.py
+-rw-r--r--   0 igo95862  (1000) igo95862  (1000)    14688 2022-07-17 20:31:32.000000 sdbus-networkmanager-2.0rc2/sdbus_block/networkmanager/enums.py
+-rw-r--r--   0 igo95862  (1000) igo95862  (1000)    17717 2022-05-28 10:24:43.000000 sdbus-networkmanager-2.0rc2/sdbus_block/networkmanager/exceptions.py
+-rw-r--r--   0 igo95862  (1000) igo95862  (1000)    29700 2022-12-26 11:11:21.000000 sdbus-networkmanager-2.0rc2/sdbus_block/networkmanager/interfaces_devices.py
+-rw-r--r--   0 igo95862  (1000) igo95862  (1000)    35524 2022-12-26 10:32:48.000000 sdbus-networkmanager-2.0rc2/sdbus_block/networkmanager/interfaces_other.py
+-rw-r--r--   0 igo95862  (1000) igo95862  (1000)    33988 2022-07-17 20:31:32.000000 sdbus-networkmanager-2.0rc2/sdbus_block/networkmanager/objects.py
+-rw-r--r--   0 igo95862  (1000) igo95862  (1000)        0 2021-07-09 14:39:32.000000 sdbus-networkmanager-2.0rc2/sdbus_block/networkmanager/py.typed
+drwxr-xr-x   0 igo95862  (1000) igo95862  (1000)        0 2023-04-23 14:33:57.164354 sdbus-networkmanager-2.0rc2/sdbus_block/networkmanager/settings/
+-rw-r--r--   0 igo95862  (1000) igo95862  (1000)     3587 2023-02-04 08:24:37.000000 sdbus-networkmanager-2.0rc2/sdbus_block/networkmanager/settings/__init__.py
+-rw-r--r--   0 igo95862  (1000) igo95862  (1000)     2023 2023-02-04 08:24:37.000000 sdbus-networkmanager-2.0rc2/sdbus_block/networkmanager/settings/adsl.py
+-rw-r--r--   0 igo95862  (1000) igo95862  (1000)     5012 2023-02-04 09:10:58.000000 sdbus-networkmanager-2.0rc2/sdbus_block/networkmanager/settings/base.py
+-rw-r--r--   0 igo95862  (1000) igo95862  (1000)      955 2023-02-04 08:24:37.000000 sdbus-networkmanager-2.0rc2/sdbus_block/networkmanager/settings/bluetooth.py
+-rw-r--r--   0 igo95862  (1000) igo95862  (1000)     1125 2023-02-04 08:24:37.000000 sdbus-networkmanager-2.0rc2/sdbus_block/networkmanager/settings/bond.py
+-rw-r--r--   0 igo95862  (1000) igo95862  (1000)      723 2023-02-04 08:24:37.000000 sdbus-networkmanager-2.0rc2/sdbus_block/networkmanager/settings/bond_port.py
+-rw-r--r--   0 igo95862  (1000) igo95862  (1000)    10117 2023-02-04 08:24:37.000000 sdbus-networkmanager-2.0rc2/sdbus_block/networkmanager/settings/bridge.py
+-rw-r--r--   0 igo95862  (1000) igo95862  (1000)     1952 2023-02-04 08:24:37.000000 sdbus-networkmanager-2.0rc2/sdbus_block/networkmanager/settings/bridge_port.py
+-rw-r--r--   0 igo95862  (1000) igo95862  (1000)     2107 2023-02-04 08:24:37.000000 sdbus-networkmanager-2.0rc2/sdbus_block/networkmanager/settings/cdma.py
+-rw-r--r--   0 igo95862  (1000) igo95862  (1000)    20276 2023-02-04 08:24:37.000000 sdbus-networkmanager-2.0rc2/sdbus_block/networkmanager/settings/connection.py
+-rw-r--r--   0 igo95862  (1000) igo95862  (1000)     7952 2022-12-03 14:35:05.000000 sdbus-networkmanager-2.0rc2/sdbus_block/networkmanager/settings/datatypes.py
+-rw-r--r--   0 igo95862  (1000) igo95862  (1000)     6660 2023-02-04 08:24:37.000000 sdbus-networkmanager-2.0rc2/sdbus_block/networkmanager/settings/dcb.py
+-rw-r--r--   0 igo95862  (1000) igo95862  (1000)      428 2023-02-04 08:24:37.000000 sdbus-networkmanager-2.0rc2/sdbus_block/networkmanager/settings/dummy.py
+-rw-r--r--   0 igo95862  (1000) igo95862  (1000)    25028 2023-02-04 08:24:37.000000 sdbus-networkmanager-2.0rc2/sdbus_block/networkmanager/settings/eapol.py
+-rw-r--r--   0 igo95862  (1000) igo95862  (1000)    11472 2023-02-04 08:24:37.000000 sdbus-networkmanager-2.0rc2/sdbus_block/networkmanager/settings/ethernet.py
+-rw-r--r--   0 igo95862  (1000) igo95862  (1000)      436 2023-02-04 08:24:37.000000 sdbus-networkmanager-2.0rc2/sdbus_block/networkmanager/settings/ethtool.py
+-rw-r--r--   0 igo95862  (1000) igo95862  (1000)      432 2023-02-04 08:24:37.000000 sdbus-networkmanager-2.0rc2/sdbus_block/networkmanager/settings/generic.py
+-rw-r--r--   0 igo95862  (1000) igo95862  (1000)     5654 2023-02-04 08:24:37.000000 sdbus-networkmanager-2.0rc2/sdbus_block/networkmanager/settings/gsm.py
+-rw-r--r--   0 igo95862  (1000) igo95862  (1000)     3065 2023-02-04 08:24:37.000000 sdbus-networkmanager-2.0rc2/sdbus_block/networkmanager/settings/hostname.py
+-rw-r--r--   0 igo95862  (1000) igo95862  (1000)     2118 2023-02-04 08:24:37.000000 sdbus-networkmanager-2.0rc2/sdbus_block/networkmanager/settings/infiniband.py
+-rw-r--r--   0 igo95862  (1000) igo95862  (1000)     4404 2023-02-04 08:24:37.000000 sdbus-networkmanager-2.0rc2/sdbus_block/networkmanager/settings/ip_tunnel.py
+-rw-r--r--   0 igo95862  (1000) igo95862  (1000)    23497 2023-02-04 08:24:37.000000 sdbus-networkmanager-2.0rc2/sdbus_block/networkmanager/settings/ipv4.py
+-rw-r--r--   0 igo95862  (1000) igo95862  (1000)    25961 2023-02-04 08:24:37.000000 sdbus-networkmanager-2.0rc2/sdbus_block/networkmanager/settings/ipv6.py
+-rw-r--r--   0 igo95862  (1000) igo95862  (1000)      723 2023-02-04 08:24:37.000000 sdbus-networkmanager-2.0rc2/sdbus_block/networkmanager/settings/lowpan.py
+-rw-r--r--   0 igo95862  (1000) igo95862  (1000)     2881 2023-02-04 08:24:37.000000 sdbus-networkmanager-2.0rc2/sdbus_block/networkmanager/settings/macsec.py
+-rw-r--r--   0 igo95862  (1000) igo95862  (1000)     1581 2023-02-04 08:24:37.000000 sdbus-networkmanager-2.0rc2/sdbus_block/networkmanager/settings/macvlan.py
+-rw-r--r--   0 igo95862  (1000) igo95862  (1000)     3993 2023-02-04 08:24:37.000000 sdbus-networkmanager-2.0rc2/sdbus_block/networkmanager/settings/match.py
+-rw-r--r--   0 igo95862  (1000) igo95862  (1000)     1296 2023-02-04 08:24:37.000000 sdbus-networkmanager-2.0rc2/sdbus_block/networkmanager/settings/olpc_mesh.py
+-rw-r--r--   0 igo95862  (1000) igo95862  (1000)     1553 2023-02-04 08:24:37.000000 sdbus-networkmanager-2.0rc2/sdbus_block/networkmanager/settings/ovs_bridge.py
+-rw-r--r--   0 igo95862  (1000) igo95862  (1000)      960 2023-02-04 08:24:37.000000 sdbus-networkmanager-2.0rc2/sdbus_block/networkmanager/settings/ovs_dpdk.py
+-rw-r--r--   0 igo95862  (1000) igo95862  (1000)      686 2023-02-04 08:24:37.000000 sdbus-networkmanager-2.0rc2/sdbus_block/networkmanager/settings/ovs_external_ids.py
+-rw-r--r--   0 igo95862  (1000) igo95862  (1000)     1242 2023-02-04 08:24:37.000000 sdbus-networkmanager-2.0rc2/sdbus_block/networkmanager/settings/ovs_interface.py
+-rw-r--r--   0 igo95862  (1000) igo95862  (1000)      737 2023-02-04 08:24:37.000000 sdbus-networkmanager-2.0rc2/sdbus_block/networkmanager/settings/ovs_patch.py
+-rw-r--r--   0 igo95862  (1000) igo95862  (1000)     1843 2023-02-04 08:24:37.000000 sdbus-networkmanager-2.0rc2/sdbus_block/networkmanager/settings/ovs_port.py
+-rw-r--r--   0 igo95862  (1000) igo95862  (1000)     5940 2023-02-04 08:24:37.000000 sdbus-networkmanager-2.0rc2/sdbus_block/networkmanager/settings/ppp.py
+-rw-r--r--   0 igo95862  (1000) igo95862  (1000)     2065 2023-02-04 08:24:37.000000 sdbus-networkmanager-2.0rc2/sdbus_block/networkmanager/settings/pppoe.py
+-rw-r--r--   0 igo95862  (1000) igo95862  (1000)    17923 2023-02-04 08:24:37.000000 sdbus-networkmanager-2.0rc2/sdbus_block/networkmanager/settings/profile.py
+-rw-r--r--   0 igo95862  (1000) igo95862  (1000)     1406 2023-02-04 08:24:37.000000 sdbus-networkmanager-2.0rc2/sdbus_block/networkmanager/settings/proxy.py
+-rw-r--r--   0 igo95862  (1000) igo95862  (1000)     1761 2023-02-04 08:24:37.000000 sdbus-networkmanager-2.0rc2/sdbus_block/networkmanager/settings/serial.py
+-rw-r--r--   0 igo95862  (1000) igo95862  (1000)     2667 2023-02-04 08:24:37.000000 sdbus-networkmanager-2.0rc2/sdbus_block/networkmanager/settings/sriov.py
+-rw-r--r--   0 igo95862  (1000) igo95862  (1000)     1673 2023-02-04 08:24:37.000000 sdbus-networkmanager-2.0rc2/sdbus_block/networkmanager/settings/tc.py
+-rw-r--r--   0 igo95862  (1000) igo95862  (1000)     5537 2023-02-04 08:24:37.000000 sdbus-networkmanager-2.0rc2/sdbus_block/networkmanager/settings/team.py
+-rw-r--r--   0 igo95862  (1000) igo95862  (1000)     2935 2023-02-04 08:24:37.000000 sdbus-networkmanager-2.0rc2/sdbus_block/networkmanager/settings/team_port.py
+-rw-r--r--   0 igo95862  (1000) igo95862  (1000)     2222 2023-02-04 08:24:37.000000 sdbus-networkmanager-2.0rc2/sdbus_block/networkmanager/settings/tun.py
+-rw-r--r--   0 igo95862  (1000) igo95862  (1000)      876 2023-02-04 08:24:37.000000 sdbus-networkmanager-2.0rc2/sdbus_block/networkmanager/settings/user.py
+-rw-r--r--   0 igo95862  (1000) igo95862  (1000)      678 2023-02-04 08:24:37.000000 sdbus-networkmanager-2.0rc2/sdbus_block/networkmanager/settings/veth.py
+-rw-r--r--   0 igo95862  (1000) igo95862  (1000)     3148 2023-02-04 08:24:37.000000 sdbus-networkmanager-2.0rc2/sdbus_block/networkmanager/settings/vlan.py
+-rw-r--r--   0 igo95862  (1000) igo95862  (1000)     2749 2023-02-04 08:24:37.000000 sdbus-networkmanager-2.0rc2/sdbus_block/networkmanager/settings/vpn.py
+-rw-r--r--   0 igo95862  (1000) igo95862  (1000)      617 2023-02-04 08:24:37.000000 sdbus-networkmanager-2.0rc2/sdbus_block/networkmanager/settings/vrf.py
+-rw-r--r--   0 igo95862  (1000) igo95862  (1000)     4529 2023-02-04 08:24:37.000000 sdbus-networkmanager-2.0rc2/sdbus_block/networkmanager/settings/vxlan.py
+-rw-r--r--   0 igo95862  (1000) igo95862  (1000)     1550 2023-02-04 08:24:37.000000 sdbus-networkmanager-2.0rc2/sdbus_block/networkmanager/settings/wifi_p2p.py
+-rw-r--r--   0 igo95862  (1000) igo95862  (1000)     1059 2023-02-04 08:24:37.000000 sdbus-networkmanager-2.0rc2/sdbus_block/networkmanager/settings/wimax.py
+-rw-r--r--   0 igo95862  (1000) igo95862  (1000)     4838 2023-02-04 08:24:37.000000 sdbus-networkmanager-2.0rc2/sdbus_block/networkmanager/settings/wireguard.py
+-rw-r--r--   0 igo95862  (1000) igo95862  (1000)    12562 2023-02-04 08:24:37.000000 sdbus-networkmanager-2.0rc2/sdbus_block/networkmanager/settings/wireless.py
+-rw-r--r--   0 igo95862  (1000) igo95862  (1000)     9087 2023-02-04 08:24:37.000000 sdbus-networkmanager-2.0rc2/sdbus_block/networkmanager/settings/wireless_security.py
+-rw-r--r--   0 igo95862  (1000) igo95862  (1000)     1802 2023-02-04 08:24:37.000000 sdbus-networkmanager-2.0rc2/sdbus_block/networkmanager/settings/wpan.py
+-rw-r--r--   0 igo95862  (1000) igo95862  (1000)     1441 2022-05-28 17:36:59.000000 sdbus-networkmanager-2.0rc2/sdbus_block/networkmanager/types.py
+drwxr-xr-x   0 igo95862  (1000) igo95862  (1000)        0 2023-04-23 14:33:57.167688 sdbus-networkmanager-2.0rc2/sdbus_networkmanager.egg-info/
+-rw-r--r--   0 igo95862  (1000) igo95862  (1000)     1868 2023-04-23 14:33:57.000000 sdbus-networkmanager-2.0rc2/sdbus_networkmanager.egg-info/PKG-INFO
+-rw-r--r--   0 igo95862  (1000) igo95862  (1000)     6157 2023-04-23 14:33:57.000000 sdbus-networkmanager-2.0rc2/sdbus_networkmanager.egg-info/SOURCES.txt
+-rw-r--r--   0 igo95862  (1000) igo95862  (1000)        1 2023-04-23 14:33:57.000000 sdbus-networkmanager-2.0rc2/sdbus_networkmanager.egg-info/dependency_links.txt
+-rw-r--r--   0 igo95862  (1000) igo95862  (1000)       14 2023-04-23 14:33:57.000000 sdbus-networkmanager-2.0rc2/sdbus_networkmanager.egg-info/requires.txt
+-rw-r--r--   0 igo95862  (1000) igo95862  (1000)       24 2023-04-23 14:33:57.000000 sdbus-networkmanager-2.0rc2/sdbus_networkmanager.egg-info/top_level.txt
+-rw-r--r--   0 igo95862  (1000) igo95862  (1000)       38 2023-04-23 14:33:57.167688 sdbus-networkmanager-2.0rc2/setup.cfg
+-rw-r--r--   0 igo95862  (1000) igo95862  (1000)     2516 2023-04-23 14:33:22.000000 sdbus-networkmanager-2.0rc2/setup.py
+drwxr-xr-x   0 igo95862  (1000) igo95862  (1000)        0 2023-04-23 14:33:57.167688 sdbus-networkmanager-2.0rc2/tests/
+-rw-r--r--   0 igo95862  (1000) igo95862  (1000)     2840 2022-12-21 18:53:35.000000 sdbus-networkmanager-2.0rc2/tests/test_settings_profile.py
```

### Comparing `sdbus-networkmanager-2.0rc1/COPYING` & `sdbus-networkmanager-2.0rc2/COPYING`

 * *Files identical despite different names*

### Comparing `sdbus-networkmanager-2.0rc1/COPYING.LESSER` & `sdbus-networkmanager-2.0rc2/COPYING.LESSER`

 * *Files identical despite different names*

### Comparing `sdbus-networkmanager-2.0rc1/PKG-INFO` & `sdbus-networkmanager-2.0rc2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sdbus-networkmanager
-Version: 2.0rc1
+Version: 2.0rc2
 Summary: NetworkManager binds for sdbus.
 Home-page: https://github.com/igo95862/python-sdbus
 Author: igo95862
 Author-email: igo95862@yandex.ru
 License: LGPL-2.1-or-later
 Project-URL: Documentation, https://python-sdbus.readthedocs.io/en/latest/
 Project-URL: Source, https://github.com/igo95862/python-sdbus/
```

### Comparing `sdbus-networkmanager-2.0rc1/README.md` & `sdbus-networkmanager-2.0rc2/README.md`

 * *Files identical despite different names*

### Comparing `sdbus-networkmanager-2.0rc1/sdbus_async/networkmanager/__init__.py` & `sdbus-networkmanager-2.0rc2/sdbus_async/networkmanager/__init__.py`

 * *Files identical despite different names*

### Comparing `sdbus-networkmanager-2.0rc1/sdbus_async/networkmanager/enums.py` & `sdbus-networkmanager-2.0rc2/sdbus_async/networkmanager/enums.py`

 * *Files identical despite different names*

### Comparing `sdbus-networkmanager-2.0rc1/sdbus_async/networkmanager/exceptions.py` & `sdbus-networkmanager-2.0rc2/sdbus_async/networkmanager/exceptions.py`

 * *Files identical despite different names*

### Comparing `sdbus-networkmanager-2.0rc1/sdbus_async/networkmanager/interfaces_devices.py` & `sdbus-networkmanager-2.0rc2/sdbus_async/networkmanager/interfaces_devices.py`

 * *Files identical despite different names*

### Comparing `sdbus-networkmanager-2.0rc1/sdbus_async/networkmanager/interfaces_other.py` & `sdbus-networkmanager-2.0rc2/sdbus_async/networkmanager/interfaces_other.py`

 * *Files identical despite different names*

### Comparing `sdbus-networkmanager-2.0rc1/sdbus_async/networkmanager/objects.py` & `sdbus-networkmanager-2.0rc2/sdbus_async/networkmanager/objects.py`

 * *Files identical despite different names*

### Comparing `sdbus-networkmanager-2.0rc1/sdbus_async/networkmanager/settings/__init__.py` & `sdbus-networkmanager-2.0rc2/sdbus_async/networkmanager/settings/__init__.py`

 * *Files identical despite different names*

### Comparing `sdbus-networkmanager-2.0rc1/sdbus_async/networkmanager/settings/adsl.py` & `sdbus-networkmanager-2.0rc2/sdbus_async/networkmanager/settings/adsl.py`

 * *Files identical despite different names*

### Comparing `sdbus-networkmanager-2.0rc1/sdbus_async/networkmanager/settings/base.py` & `sdbus-networkmanager-2.0rc2/sdbus_async/networkmanager/settings/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -78,18 +78,23 @@
     @classmethod
     def from_dbus(
         cls,
         dbus_dict: NetworkManagerSettingsDomain,
     ) -> NetworkManagerSettingsMixin:
         """TODO: Add proper docstring"""
         reverse_mapping = cls.setting_name_reverse_mapping()
-        unvarianted_options = {
-            reverse_mapping[k]: cls._unpack_variant(k, *v)
-            for k, v in dbus_dict.items()
-        }
+        unvarianted_options = {}
+        for k, v in dbus_dict.items():
+            try:
+                reverse_name = reverse_mapping[k]
+            except KeyError:
+                continue
+
+            unvarianted_options[reverse_name] = cls._unpack_variant(k, *v)
+
         return cls(**unvarianted_options)
 
     @classmethod
     def from_dict(cls,
                   plain_dict: Dict[str, Any]
                   ) -> NetworkManagerSettingsMixin:
         options = {}
```

### Comparing `sdbus-networkmanager-2.0rc1/sdbus_async/networkmanager/settings/bluetooth.py` & `sdbus-networkmanager-2.0rc2/sdbus_async/networkmanager/settings/bluetooth.py`

 * *Files identical despite different names*

### Comparing `sdbus-networkmanager-2.0rc1/sdbus_async/networkmanager/settings/bond.py` & `sdbus-networkmanager-2.0rc2/sdbus_async/networkmanager/settings/bond.py`

 * *Files identical despite different names*

### Comparing `sdbus-networkmanager-2.0rc1/sdbus_async/networkmanager/settings/bond_port.py` & `sdbus-networkmanager-2.0rc2/sdbus_async/networkmanager/settings/bond_port.py`

 * *Files identical despite different names*

### Comparing `sdbus-networkmanager-2.0rc1/sdbus_async/networkmanager/settings/bridge.py` & `sdbus-networkmanager-2.0rc2/sdbus_async/networkmanager/settings/bridge.py`

 * *Files identical despite different names*

### Comparing `sdbus-networkmanager-2.0rc1/sdbus_async/networkmanager/settings/bridge_port.py` & `sdbus-networkmanager-2.0rc2/sdbus_async/networkmanager/settings/bridge_port.py`

 * *Files identical despite different names*

### Comparing `sdbus-networkmanager-2.0rc1/sdbus_async/networkmanager/settings/cdma.py` & `sdbus-networkmanager-2.0rc2/sdbus_async/networkmanager/settings/cdma.py`

 * *Files identical despite different names*

### Comparing `sdbus-networkmanager-2.0rc1/sdbus_async/networkmanager/settings/connection.py` & `sdbus-networkmanager-2.0rc2/sdbus_async/networkmanager/settings/connection.py`

 * *Files identical despite different names*

### Comparing `sdbus-networkmanager-2.0rc1/sdbus_async/networkmanager/settings/datatypes.py` & `sdbus-networkmanager-2.0rc2/sdbus_async/networkmanager/settings/datatypes.py`

 * *Files identical despite different names*

### Comparing `sdbus-networkmanager-2.0rc1/sdbus_async/networkmanager/settings/dcb.py` & `sdbus-networkmanager-2.0rc2/sdbus_async/networkmanager/settings/dcb.py`

 * *Files identical despite different names*

### Comparing `sdbus-networkmanager-2.0rc1/sdbus_async/networkmanager/settings/eapol.py` & `sdbus-networkmanager-2.0rc2/sdbus_async/networkmanager/settings/eapol.py`

 * *Files identical despite different names*

### Comparing `sdbus-networkmanager-2.0rc1/sdbus_async/networkmanager/settings/ethernet.py` & `sdbus-networkmanager-2.0rc2/sdbus_async/networkmanager/settings/ethernet.py`

 * *Files identical despite different names*

### Comparing `sdbus-networkmanager-2.0rc1/sdbus_async/networkmanager/settings/gsm.py` & `sdbus-networkmanager-2.0rc2/sdbus_async/networkmanager/settings/gsm.py`

 * *Files identical despite different names*

### Comparing `sdbus-networkmanager-2.0rc1/sdbus_async/networkmanager/settings/hostname.py` & `sdbus-networkmanager-2.0rc2/sdbus_async/networkmanager/settings/hostname.py`

 * *Files identical despite different names*

### Comparing `sdbus-networkmanager-2.0rc1/sdbus_async/networkmanager/settings/infiniband.py` & `sdbus-networkmanager-2.0rc2/sdbus_async/networkmanager/settings/infiniband.py`

 * *Files identical despite different names*

### Comparing `sdbus-networkmanager-2.0rc1/sdbus_async/networkmanager/settings/ip_tunnel.py` & `sdbus-networkmanager-2.0rc2/sdbus_async/networkmanager/settings/ip_tunnel.py`

 * *Files identical despite different names*

### Comparing `sdbus-networkmanager-2.0rc1/sdbus_async/networkmanager/settings/ipv4.py` & `sdbus-networkmanager-2.0rc2/sdbus_async/networkmanager/settings/ipv4.py`

 * *Files identical despite different names*

### Comparing `sdbus-networkmanager-2.0rc1/sdbus_async/networkmanager/settings/ipv6.py` & `sdbus-networkmanager-2.0rc2/sdbus_async/networkmanager/settings/ipv6.py`

 * *Files identical despite different names*

### Comparing `sdbus-networkmanager-2.0rc1/sdbus_async/networkmanager/settings/lowpan.py` & `sdbus-networkmanager-2.0rc2/sdbus_async/networkmanager/settings/lowpan.py`

 * *Files identical despite different names*

### Comparing `sdbus-networkmanager-2.0rc1/sdbus_async/networkmanager/settings/macsec.py` & `sdbus-networkmanager-2.0rc2/sdbus_async/networkmanager/settings/macsec.py`

 * *Files identical despite different names*

### Comparing `sdbus-networkmanager-2.0rc1/sdbus_async/networkmanager/settings/macvlan.py` & `sdbus-networkmanager-2.0rc2/sdbus_async/networkmanager/settings/macvlan.py`

 * *Files identical despite different names*

### Comparing `sdbus-networkmanager-2.0rc1/sdbus_async/networkmanager/settings/match.py` & `sdbus-networkmanager-2.0rc2/sdbus_async/networkmanager/settings/match.py`

 * *Files identical despite different names*

### Comparing `sdbus-networkmanager-2.0rc1/sdbus_async/networkmanager/settings/olpc_mesh.py` & `sdbus-networkmanager-2.0rc2/sdbus_async/networkmanager/settings/olpc_mesh.py`

 * *Files identical despite different names*

### Comparing `sdbus-networkmanager-2.0rc1/sdbus_async/networkmanager/settings/ovs_bridge.py` & `sdbus-networkmanager-2.0rc2/sdbus_async/networkmanager/settings/ovs_bridge.py`

 * *Files identical despite different names*

### Comparing `sdbus-networkmanager-2.0rc1/sdbus_async/networkmanager/settings/ovs_dpdk.py` & `sdbus-networkmanager-2.0rc2/sdbus_async/networkmanager/settings/ovs_dpdk.py`

 * *Files identical despite different names*

### Comparing `sdbus-networkmanager-2.0rc1/sdbus_async/networkmanager/settings/ovs_external_ids.py` & `sdbus-networkmanager-2.0rc2/sdbus_async/networkmanager/settings/ovs_external_ids.py`

 * *Files identical despite different names*

### Comparing `sdbus-networkmanager-2.0rc1/sdbus_async/networkmanager/settings/ovs_interface.py` & `sdbus-networkmanager-2.0rc2/sdbus_async/networkmanager/settings/ovs_interface.py`

 * *Files identical despite different names*

### Comparing `sdbus-networkmanager-2.0rc1/sdbus_async/networkmanager/settings/ovs_patch.py` & `sdbus-networkmanager-2.0rc2/sdbus_async/networkmanager/settings/ovs_patch.py`

 * *Files identical despite different names*

### Comparing `sdbus-networkmanager-2.0rc1/sdbus_async/networkmanager/settings/ovs_port.py` & `sdbus-networkmanager-2.0rc2/sdbus_async/networkmanager/settings/ovs_port.py`

 * *Files identical despite different names*

### Comparing `sdbus-networkmanager-2.0rc1/sdbus_async/networkmanager/settings/ppp.py` & `sdbus-networkmanager-2.0rc2/sdbus_async/networkmanager/settings/ppp.py`

 * *Files identical despite different names*

### Comparing `sdbus-networkmanager-2.0rc1/sdbus_async/networkmanager/settings/pppoe.py` & `sdbus-networkmanager-2.0rc2/sdbus_async/networkmanager/settings/pppoe.py`

 * *Files identical despite different names*

### Comparing `sdbus-networkmanager-2.0rc1/sdbus_async/networkmanager/settings/profile.py` & `sdbus-networkmanager-2.0rc2/sdbus_async/networkmanager/settings/profile.py`

 * *Files identical despite different names*

### Comparing `sdbus-networkmanager-2.0rc1/sdbus_async/networkmanager/settings/proxy.py` & `sdbus-networkmanager-2.0rc2/sdbus_async/networkmanager/settings/proxy.py`

 * *Files identical despite different names*

### Comparing `sdbus-networkmanager-2.0rc1/sdbus_async/networkmanager/settings/serial.py` & `sdbus-networkmanager-2.0rc2/sdbus_async/networkmanager/settings/serial.py`

 * *Files identical despite different names*

### Comparing `sdbus-networkmanager-2.0rc1/sdbus_async/networkmanager/settings/sriov.py` & `sdbus-networkmanager-2.0rc2/sdbus_async/networkmanager/settings/sriov.py`

 * *Files identical despite different names*

### Comparing `sdbus-networkmanager-2.0rc1/sdbus_async/networkmanager/settings/tc.py` & `sdbus-networkmanager-2.0rc2/sdbus_async/networkmanager/settings/tc.py`

 * *Files identical despite different names*

### Comparing `sdbus-networkmanager-2.0rc1/sdbus_async/networkmanager/settings/team.py` & `sdbus-networkmanager-2.0rc2/sdbus_async/networkmanager/settings/team.py`

 * *Files identical despite different names*

### Comparing `sdbus-networkmanager-2.0rc1/sdbus_async/networkmanager/settings/team_port.py` & `sdbus-networkmanager-2.0rc2/sdbus_async/networkmanager/settings/team_port.py`

 * *Files identical despite different names*

### Comparing `sdbus-networkmanager-2.0rc1/sdbus_async/networkmanager/settings/tun.py` & `sdbus-networkmanager-2.0rc2/sdbus_async/networkmanager/settings/tun.py`

 * *Files identical despite different names*

### Comparing `sdbus-networkmanager-2.0rc1/sdbus_async/networkmanager/settings/user.py` & `sdbus-networkmanager-2.0rc2/sdbus_async/networkmanager/settings/user.py`

 * *Files identical despite different names*

### Comparing `sdbus-networkmanager-2.0rc1/sdbus_async/networkmanager/settings/veth.py` & `sdbus-networkmanager-2.0rc2/sdbus_async/networkmanager/settings/veth.py`

 * *Files identical despite different names*

### Comparing `sdbus-networkmanager-2.0rc1/sdbus_async/networkmanager/settings/vlan.py` & `sdbus-networkmanager-2.0rc2/sdbus_async/networkmanager/settings/vlan.py`

 * *Files identical despite different names*

### Comparing `sdbus-networkmanager-2.0rc1/sdbus_async/networkmanager/settings/vpn.py` & `sdbus-networkmanager-2.0rc2/sdbus_async/networkmanager/settings/vpn.py`

 * *Files identical despite different names*

### Comparing `sdbus-networkmanager-2.0rc1/sdbus_async/networkmanager/settings/vrf.py` & `sdbus-networkmanager-2.0rc2/sdbus_async/networkmanager/settings/vrf.py`

 * *Files identical despite different names*

### Comparing `sdbus-networkmanager-2.0rc1/sdbus_async/networkmanager/settings/vxlan.py` & `sdbus-networkmanager-2.0rc2/sdbus_async/networkmanager/settings/vxlan.py`

 * *Files identical despite different names*

### Comparing `sdbus-networkmanager-2.0rc1/sdbus_async/networkmanager/settings/wifi_p2p.py` & `sdbus-networkmanager-2.0rc2/sdbus_async/networkmanager/settings/wifi_p2p.py`

 * *Files identical despite different names*

### Comparing `sdbus-networkmanager-2.0rc1/sdbus_async/networkmanager/settings/wimax.py` & `sdbus-networkmanager-2.0rc2/sdbus_async/networkmanager/settings/wimax.py`

 * *Files identical despite different names*

### Comparing `sdbus-networkmanager-2.0rc1/sdbus_async/networkmanager/settings/wireguard.py` & `sdbus-networkmanager-2.0rc2/sdbus_async/networkmanager/settings/wireguard.py`

 * *Files identical despite different names*

### Comparing `sdbus-networkmanager-2.0rc1/sdbus_async/networkmanager/settings/wireless.py` & `sdbus-networkmanager-2.0rc2/sdbus_async/networkmanager/settings/wireless.py`

 * *Files identical despite different names*

### Comparing `sdbus-networkmanager-2.0rc1/sdbus_async/networkmanager/settings/wireless_security.py` & `sdbus-networkmanager-2.0rc2/sdbus_async/networkmanager/settings/wireless_security.py`

 * *Files identical despite different names*

### Comparing `sdbus-networkmanager-2.0rc1/sdbus_async/networkmanager/settings/wpan.py` & `sdbus-networkmanager-2.0rc2/sdbus_async/networkmanager/settings/wpan.py`

 * *Files identical despite different names*

### Comparing `sdbus-networkmanager-2.0rc1/sdbus_async/networkmanager/types.py` & `sdbus-networkmanager-2.0rc2/sdbus_async/networkmanager/types.py`

 * *Files identical despite different names*

### Comparing `sdbus-networkmanager-2.0rc1/sdbus_block/networkmanager/__init__.py` & `sdbus-networkmanager-2.0rc2/sdbus_block/networkmanager/__init__.py`

 * *Files identical despite different names*

### Comparing `sdbus-networkmanager-2.0rc1/sdbus_block/networkmanager/enums.py` & `sdbus-networkmanager-2.0rc2/sdbus_block/networkmanager/enums.py`

 * *Files identical despite different names*

### Comparing `sdbus-networkmanager-2.0rc1/sdbus_block/networkmanager/exceptions.py` & `sdbus-networkmanager-2.0rc2/sdbus_block/networkmanager/exceptions.py`

 * *Files identical despite different names*

### Comparing `sdbus-networkmanager-2.0rc1/sdbus_block/networkmanager/interfaces_devices.py` & `sdbus-networkmanager-2.0rc2/sdbus_block/networkmanager/interfaces_devices.py`

 * *Files identical despite different names*

### Comparing `sdbus-networkmanager-2.0rc1/sdbus_block/networkmanager/interfaces_other.py` & `sdbus-networkmanager-2.0rc2/sdbus_block/networkmanager/interfaces_other.py`

 * *Files identical despite different names*

### Comparing `sdbus-networkmanager-2.0rc1/sdbus_block/networkmanager/objects.py` & `sdbus-networkmanager-2.0rc2/sdbus_block/networkmanager/objects.py`

 * *Files identical despite different names*

### Comparing `sdbus-networkmanager-2.0rc1/sdbus_block/networkmanager/settings/__init__.py` & `sdbus-networkmanager-2.0rc2/sdbus_block/networkmanager/settings/__init__.py`

 * *Files identical despite different names*

### Comparing `sdbus-networkmanager-2.0rc1/sdbus_block/networkmanager/settings/adsl.py` & `sdbus-networkmanager-2.0rc2/sdbus_block/networkmanager/settings/adsl.py`

 * *Files identical despite different names*

### Comparing `sdbus-networkmanager-2.0rc1/sdbus_block/networkmanager/settings/base.py` & `sdbus-networkmanager-2.0rc2/sdbus_block/networkmanager/settings/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -78,18 +78,23 @@
     @classmethod
     def from_dbus(
         cls,
         dbus_dict: NetworkManagerSettingsDomain,
     ) -> NetworkManagerSettingsMixin:
         """TODO: Add proper docstring"""
         reverse_mapping = cls.setting_name_reverse_mapping()
-        unvarianted_options = {
-            reverse_mapping[k]: cls._unpack_variant(k, *v)
-            for k, v in dbus_dict.items()
-        }
+        unvarianted_options = {}
+        for k, v in dbus_dict.items():
+            try:
+                reverse_name = reverse_mapping[k]
+            except KeyError:
+                continue
+
+            unvarianted_options[reverse_name] = cls._unpack_variant(k, *v)
+
         return cls(**unvarianted_options)
 
     @classmethod
     def from_dict(cls,
                   plain_dict: Dict[str, Any]
                   ) -> NetworkManagerSettingsMixin:
         options = {}
```

### Comparing `sdbus-networkmanager-2.0rc1/sdbus_block/networkmanager/settings/bluetooth.py` & `sdbus-networkmanager-2.0rc2/sdbus_block/networkmanager/settings/bluetooth.py`

 * *Files identical despite different names*

### Comparing `sdbus-networkmanager-2.0rc1/sdbus_block/networkmanager/settings/bond.py` & `sdbus-networkmanager-2.0rc2/sdbus_block/networkmanager/settings/bond.py`

 * *Files identical despite different names*

### Comparing `sdbus-networkmanager-2.0rc1/sdbus_block/networkmanager/settings/bond_port.py` & `sdbus-networkmanager-2.0rc2/sdbus_block/networkmanager/settings/bond_port.py`

 * *Files identical despite different names*

### Comparing `sdbus-networkmanager-2.0rc1/sdbus_block/networkmanager/settings/bridge.py` & `sdbus-networkmanager-2.0rc2/sdbus_block/networkmanager/settings/bridge.py`

 * *Files identical despite different names*

### Comparing `sdbus-networkmanager-2.0rc1/sdbus_block/networkmanager/settings/bridge_port.py` & `sdbus-networkmanager-2.0rc2/sdbus_block/networkmanager/settings/bridge_port.py`

 * *Files identical despite different names*

### Comparing `sdbus-networkmanager-2.0rc1/sdbus_block/networkmanager/settings/cdma.py` & `sdbus-networkmanager-2.0rc2/sdbus_block/networkmanager/settings/cdma.py`

 * *Files identical despite different names*

### Comparing `sdbus-networkmanager-2.0rc1/sdbus_block/networkmanager/settings/connection.py` & `sdbus-networkmanager-2.0rc2/sdbus_block/networkmanager/settings/connection.py`

 * *Files identical despite different names*

### Comparing `sdbus-networkmanager-2.0rc1/sdbus_block/networkmanager/settings/datatypes.py` & `sdbus-networkmanager-2.0rc2/sdbus_block/networkmanager/settings/datatypes.py`

 * *Files identical despite different names*

### Comparing `sdbus-networkmanager-2.0rc1/sdbus_block/networkmanager/settings/dcb.py` & `sdbus-networkmanager-2.0rc2/sdbus_block/networkmanager/settings/dcb.py`

 * *Files identical despite different names*

### Comparing `sdbus-networkmanager-2.0rc1/sdbus_block/networkmanager/settings/eapol.py` & `sdbus-networkmanager-2.0rc2/sdbus_block/networkmanager/settings/eapol.py`

 * *Files identical despite different names*

### Comparing `sdbus-networkmanager-2.0rc1/sdbus_block/networkmanager/settings/ethernet.py` & `sdbus-networkmanager-2.0rc2/sdbus_block/networkmanager/settings/ethernet.py`

 * *Files identical despite different names*

### Comparing `sdbus-networkmanager-2.0rc1/sdbus_block/networkmanager/settings/gsm.py` & `sdbus-networkmanager-2.0rc2/sdbus_block/networkmanager/settings/gsm.py`

 * *Files identical despite different names*

### Comparing `sdbus-networkmanager-2.0rc1/sdbus_block/networkmanager/settings/hostname.py` & `sdbus-networkmanager-2.0rc2/sdbus_block/networkmanager/settings/hostname.py`

 * *Files identical despite different names*

### Comparing `sdbus-networkmanager-2.0rc1/sdbus_block/networkmanager/settings/infiniband.py` & `sdbus-networkmanager-2.0rc2/sdbus_block/networkmanager/settings/infiniband.py`

 * *Files identical despite different names*

### Comparing `sdbus-networkmanager-2.0rc1/sdbus_block/networkmanager/settings/ip_tunnel.py` & `sdbus-networkmanager-2.0rc2/sdbus_block/networkmanager/settings/ip_tunnel.py`

 * *Files identical despite different names*

### Comparing `sdbus-networkmanager-2.0rc1/sdbus_block/networkmanager/settings/ipv4.py` & `sdbus-networkmanager-2.0rc2/sdbus_block/networkmanager/settings/ipv4.py`

 * *Files identical despite different names*

### Comparing `sdbus-networkmanager-2.0rc1/sdbus_block/networkmanager/settings/ipv6.py` & `sdbus-networkmanager-2.0rc2/sdbus_block/networkmanager/settings/ipv6.py`

 * *Files identical despite different names*

### Comparing `sdbus-networkmanager-2.0rc1/sdbus_block/networkmanager/settings/lowpan.py` & `sdbus-networkmanager-2.0rc2/sdbus_block/networkmanager/settings/lowpan.py`

 * *Files identical despite different names*

### Comparing `sdbus-networkmanager-2.0rc1/sdbus_block/networkmanager/settings/macsec.py` & `sdbus-networkmanager-2.0rc2/sdbus_block/networkmanager/settings/macsec.py`

 * *Files identical despite different names*

### Comparing `sdbus-networkmanager-2.0rc1/sdbus_block/networkmanager/settings/macvlan.py` & `sdbus-networkmanager-2.0rc2/sdbus_block/networkmanager/settings/macvlan.py`

 * *Files identical despite different names*

### Comparing `sdbus-networkmanager-2.0rc1/sdbus_block/networkmanager/settings/match.py` & `sdbus-networkmanager-2.0rc2/sdbus_block/networkmanager/settings/match.py`

 * *Files identical despite different names*

### Comparing `sdbus-networkmanager-2.0rc1/sdbus_block/networkmanager/settings/olpc_mesh.py` & `sdbus-networkmanager-2.0rc2/sdbus_block/networkmanager/settings/olpc_mesh.py`

 * *Files identical despite different names*

### Comparing `sdbus-networkmanager-2.0rc1/sdbus_block/networkmanager/settings/ovs_bridge.py` & `sdbus-networkmanager-2.0rc2/sdbus_block/networkmanager/settings/ovs_bridge.py`

 * *Files identical despite different names*

### Comparing `sdbus-networkmanager-2.0rc1/sdbus_block/networkmanager/settings/ovs_dpdk.py` & `sdbus-networkmanager-2.0rc2/sdbus_block/networkmanager/settings/ovs_dpdk.py`

 * *Files identical despite different names*

### Comparing `sdbus-networkmanager-2.0rc1/sdbus_block/networkmanager/settings/ovs_external_ids.py` & `sdbus-networkmanager-2.0rc2/sdbus_block/networkmanager/settings/ovs_external_ids.py`

 * *Files identical despite different names*

### Comparing `sdbus-networkmanager-2.0rc1/sdbus_block/networkmanager/settings/ovs_interface.py` & `sdbus-networkmanager-2.0rc2/sdbus_block/networkmanager/settings/ovs_interface.py`

 * *Files identical despite different names*

### Comparing `sdbus-networkmanager-2.0rc1/sdbus_block/networkmanager/settings/ovs_patch.py` & `sdbus-networkmanager-2.0rc2/sdbus_block/networkmanager/settings/ovs_patch.py`

 * *Files identical despite different names*

### Comparing `sdbus-networkmanager-2.0rc1/sdbus_block/networkmanager/settings/ovs_port.py` & `sdbus-networkmanager-2.0rc2/sdbus_block/networkmanager/settings/ovs_port.py`

 * *Files identical despite different names*

### Comparing `sdbus-networkmanager-2.0rc1/sdbus_block/networkmanager/settings/ppp.py` & `sdbus-networkmanager-2.0rc2/sdbus_block/networkmanager/settings/ppp.py`

 * *Files identical despite different names*

### Comparing `sdbus-networkmanager-2.0rc1/sdbus_block/networkmanager/settings/pppoe.py` & `sdbus-networkmanager-2.0rc2/sdbus_block/networkmanager/settings/pppoe.py`

 * *Files identical despite different names*

### Comparing `sdbus-networkmanager-2.0rc1/sdbus_block/networkmanager/settings/profile.py` & `sdbus-networkmanager-2.0rc2/sdbus_block/networkmanager/settings/profile.py`

 * *Files identical despite different names*

### Comparing `sdbus-networkmanager-2.0rc1/sdbus_block/networkmanager/settings/proxy.py` & `sdbus-networkmanager-2.0rc2/sdbus_block/networkmanager/settings/proxy.py`

 * *Files identical despite different names*

### Comparing `sdbus-networkmanager-2.0rc1/sdbus_block/networkmanager/settings/serial.py` & `sdbus-networkmanager-2.0rc2/sdbus_block/networkmanager/settings/serial.py`

 * *Files identical despite different names*

### Comparing `sdbus-networkmanager-2.0rc1/sdbus_block/networkmanager/settings/sriov.py` & `sdbus-networkmanager-2.0rc2/sdbus_block/networkmanager/settings/sriov.py`

 * *Files identical despite different names*

### Comparing `sdbus-networkmanager-2.0rc1/sdbus_block/networkmanager/settings/tc.py` & `sdbus-networkmanager-2.0rc2/sdbus_block/networkmanager/settings/tc.py`

 * *Files identical despite different names*

### Comparing `sdbus-networkmanager-2.0rc1/sdbus_block/networkmanager/settings/team.py` & `sdbus-networkmanager-2.0rc2/sdbus_block/networkmanager/settings/team.py`

 * *Files identical despite different names*

### Comparing `sdbus-networkmanager-2.0rc1/sdbus_block/networkmanager/settings/team_port.py` & `sdbus-networkmanager-2.0rc2/sdbus_block/networkmanager/settings/team_port.py`

 * *Files identical despite different names*

### Comparing `sdbus-networkmanager-2.0rc1/sdbus_block/networkmanager/settings/tun.py` & `sdbus-networkmanager-2.0rc2/sdbus_block/networkmanager/settings/tun.py`

 * *Files identical despite different names*

### Comparing `sdbus-networkmanager-2.0rc1/sdbus_block/networkmanager/settings/user.py` & `sdbus-networkmanager-2.0rc2/sdbus_block/networkmanager/settings/user.py`

 * *Files identical despite different names*

### Comparing `sdbus-networkmanager-2.0rc1/sdbus_block/networkmanager/settings/veth.py` & `sdbus-networkmanager-2.0rc2/sdbus_block/networkmanager/settings/veth.py`

 * *Files identical despite different names*

### Comparing `sdbus-networkmanager-2.0rc1/sdbus_block/networkmanager/settings/vlan.py` & `sdbus-networkmanager-2.0rc2/sdbus_block/networkmanager/settings/vlan.py`

 * *Files identical despite different names*

### Comparing `sdbus-networkmanager-2.0rc1/sdbus_block/networkmanager/settings/vpn.py` & `sdbus-networkmanager-2.0rc2/sdbus_block/networkmanager/settings/vpn.py`

 * *Files identical despite different names*

### Comparing `sdbus-networkmanager-2.0rc1/sdbus_block/networkmanager/settings/vrf.py` & `sdbus-networkmanager-2.0rc2/sdbus_block/networkmanager/settings/vrf.py`

 * *Files identical despite different names*

### Comparing `sdbus-networkmanager-2.0rc1/sdbus_block/networkmanager/settings/vxlan.py` & `sdbus-networkmanager-2.0rc2/sdbus_block/networkmanager/settings/vxlan.py`

 * *Files identical despite different names*

### Comparing `sdbus-networkmanager-2.0rc1/sdbus_block/networkmanager/settings/wifi_p2p.py` & `sdbus-networkmanager-2.0rc2/sdbus_block/networkmanager/settings/wifi_p2p.py`

 * *Files identical despite different names*

### Comparing `sdbus-networkmanager-2.0rc1/sdbus_block/networkmanager/settings/wimax.py` & `sdbus-networkmanager-2.0rc2/sdbus_block/networkmanager/settings/wimax.py`

 * *Files identical despite different names*

### Comparing `sdbus-networkmanager-2.0rc1/sdbus_block/networkmanager/settings/wireguard.py` & `sdbus-networkmanager-2.0rc2/sdbus_block/networkmanager/settings/wireguard.py`

 * *Files identical despite different names*

### Comparing `sdbus-networkmanager-2.0rc1/sdbus_block/networkmanager/settings/wireless.py` & `sdbus-networkmanager-2.0rc2/sdbus_block/networkmanager/settings/wireless.py`

 * *Files identical despite different names*

### Comparing `sdbus-networkmanager-2.0rc1/sdbus_block/networkmanager/settings/wireless_security.py` & `sdbus-networkmanager-2.0rc2/sdbus_block/networkmanager/settings/wireless_security.py`

 * *Files identical despite different names*

### Comparing `sdbus-networkmanager-2.0rc1/sdbus_block/networkmanager/settings/wpan.py` & `sdbus-networkmanager-2.0rc2/sdbus_block/networkmanager/settings/wpan.py`

 * *Files identical despite different names*

### Comparing `sdbus-networkmanager-2.0rc1/sdbus_block/networkmanager/types.py` & `sdbus-networkmanager-2.0rc2/sdbus_block/networkmanager/types.py`

 * *Files identical despite different names*

### Comparing `sdbus-networkmanager-2.0rc1/sdbus_networkmanager.egg-info/PKG-INFO` & `sdbus-networkmanager-2.0rc2/sdbus_networkmanager.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sdbus-networkmanager
-Version: 2.0rc1
+Version: 2.0rc2
 Summary: NetworkManager binds for sdbus.
 Home-page: https://github.com/igo95862/python-sdbus
 Author: igo95862
 Author-email: igo95862@yandex.ru
 License: LGPL-2.1-or-later
 Project-URL: Documentation, https://python-sdbus.readthedocs.io/en/latest/
 Project-URL: Source, https://github.com/igo95862/python-sdbus/
```

### Comparing `sdbus-networkmanager-2.0rc1/sdbus_networkmanager.egg-info/SOURCES.txt` & `sdbus-networkmanager-2.0rc2/sdbus_networkmanager.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -130,8 +130,9 @@
 sdbus_block/networkmanager/settings/wireless.py
 sdbus_block/networkmanager/settings/wireless_security.py
 sdbus_block/networkmanager/settings/wpan.py
 sdbus_networkmanager.egg-info/PKG-INFO
 sdbus_networkmanager.egg-info/SOURCES.txt
 sdbus_networkmanager.egg-info/dependency_links.txt
 sdbus_networkmanager.egg-info/requires.txt
-sdbus_networkmanager.egg-info/top_level.txt
+sdbus_networkmanager.egg-info/top_level.txt
+tests/test_settings_profile.py
```

### Comparing `sdbus-networkmanager-2.0rc1/setup.py` & `sdbus-networkmanager-2.0rc2/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -25,15 +25,15 @@
     long_description = f.read()
 
 setup(
     name='sdbus-networkmanager',
     description=('NetworkManager binds for sdbus.'),
     long_description=long_description,
     long_description_content_type='text/markdown',
-    version='2.0rc1',
+    version='2.0rc2',
     url='https://github.com/igo95862/python-sdbus',
     author='igo95862',
     author_email='igo95862@yandex.ru',
     license='LGPL-2.1-or-later',
     keywords='dbus networkmanager networking linux freedesktop',
     project_urls={
         'Documentation': 'https://python-sdbus.readthedocs.io/en/latest/',
```

