python-firewall-mapper
----------------------

This is a very simple script to help you map tcp/udp port rules, to try and
find a valid communications channel to the outside world when testing a
local network.


Usage:

On the external server:

./python-firewall-mapper [-i INTERFACE | -l ADDRESS]


In the local network:

for PORT in `seq 1 65535`; do echo test | nc $REMOTE_IP $PORT; done

(or any other bash trickery you can think of)



