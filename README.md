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
