# CS-4390-ICMP-Pinger

The task is to develop your own Ping application in Python. Your application will use ICMP but, in 
order to keep it simple, will not exactly follow the official specification in RFC 1739. Note that you 
will only need to write the client side of the program, as the functionality needed on the server side 
is built into almost all operating systems.
The client sends ping requests to a specified host separated by approximately one second. Each 
message contains a payload of data that includes a timestamp. After sending each packet, the 
application waits up to one second to receive a reply. If one second goes by without a reply from the 
server, then the client assumes that either the ping packet or the pong packet was lost in the 
network (or that the server is down)
Once you have filled in the gaps, the code should be able to send three pings to each of the following 
servers:
localhost
google.com
utexas.edu
www.u-tokyo.ac.jp
telecom-paris.fr
When the pinger receives a reply, it should print the IP address of the host that replied, the number 
of bytes in the reply, the time elapsed, and the TTL of the reply

adding the following extensions
1) The code maintains statistics on the number of pings sent, the number of pongs received, the 
number of losses, and the loss percentage, and prints the result at the end of each ping session with
a server:
2) The code maintains statistics on the average, minimum and maximum delays and prints the result 
at the end of each ping session with a server (this should be done only if there was at least one pong)
