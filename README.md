systemtap-network-monitor
=========================

A network connection monitor using the systemtap interface to also identify the
PID of the connection.

This is useful for logging anomalies of outgoing traffic. It can be used as a
sort of host monitoring system.

In the tags file various types of tags can be specified in order to tag well
known, applications, ips, etc. Entries that are not tagged will be logged in red
coloring, so that they stand out.

* Needs GeoCity Database from http://dev.maxmind.com/geoip/geolite in the same
  directory called GeoLiteCity.dat
* Needs systemtap-1.8
* Needs debugging symbols installed for systemtap. Here is an easy howto:
  http://sourceware.org/systemtap/wiki/SystemtapOnUbuntu

After that just run ./pinemo with root privileges
