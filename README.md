munin-tor
=========

Muin plugins to monitor Tor node

2 very simple Munin plugins for Tor

Installation
~~~~~~~~~~~~

For Debian / Ubuntu :
-  Save tor_sys and tor_connections in /usr/share/munin/plugins/
-  Create 2 symbolic links in /etc/munin/plugins
   ``ln -s /usr/share/munin/plugins/tor_sys /etc/munin/plugins/tor_sys``
   ``ln -s /usr/share/munin/plugins/tor_connections /etc/munin/plugins/tor_connections``
-  Add this 2 lines at the end of /etc/munin/plugin-conf.d/munin-node
   [tor_*]
   user root
-  Restart munin-node service
   ``service munin-node restart``
