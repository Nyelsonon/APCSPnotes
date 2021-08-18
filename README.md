# APCSPnotes

|| What is bandwidth?
-	The capacity of data transfer in a system. Measured by bitrate.
|| What is bitrate?
-	The number of bits a system can send per second.
|| What is latency?
-	The time it takes for a bit to travel from sender to receiver

| Sending Information:

|| How do computers find each other?
-	Computers find other computers through addressing.
-	Every device has its own unique address.
-	Data sent has a to address as well as a from address.
-	All addresses follow a certain standard.
-	The Internet Protocol (IP)
-	IP addresses are 4 numbers
-	Ex: 93.184.216.34
-	1st num = network 
-	2nd num = 

|| How to give human readable names to IP Addresses?
-	Websites register a name
-	DNS maps domains to IP address
google.com -> 172.217.18.174

|| How to request resources off the web?(DNS System)
-	DNS translates name to IP.
-	Check memory(cache) to see if address is already existing.
-	Find where com lives, ask root server where com is.
-	Return IP address for com server.
-	Asks com where to find requested name.
-	Returns IP address for name in com.
-	Asks where www is.
-	Returns address.
-	IP address is complete, can request to website server.
-	Dynamic IP: If a server has too much traffic the IP can change(smart DNS).
-	This hierarchy makes the DNS system scalable
-	Allows for items to be added easily
-	Easier to search in the hierarchy rather than the entire internet

|| How do we make information get to a destination?
-	Routing
-	Routing is set by router
-	Rather than making individual connections, put router
-	Every computer is connected by a router
-	Two computers on the internet are connected through routers
-	Looks through all routers, finds router path with lowest cost(lowest distance, highest speed, lowest risk)
-	Multiple paths exist through two points
-	Internet is fault tolerant
-	Is hard to break

|| Packets

-	Data is broken into packets
-	Once packets arrive they are pieced together
-	The format of a packet is defined by a protocol
-	All packets must have a destination address, and a from address
-	To send multiple packets we need the TCP protocol
-	Checks if all packets made to destination and were pieced together
-	Metadata: tells order of packets
-	Packets are labeled with metadata
