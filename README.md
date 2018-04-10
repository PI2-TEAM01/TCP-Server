Without going in the details :

Before communicate between the Server and the Client, we need the Server and the Client to have fixed IP.

The "conn_ap" will be responsible of the connection of the server to the access point :
That's why we need to specify in the conn_ap.h

* SSID
* Password

of the access point

Then when we are connected, the DHCP of the access point will give an IP for our server

The server doesn't need to know the IP of the client.

Then when we'll be connected, we will use the "TCP_Server.c" to communicate between the two :

 * TCPLocalServer : that set the server and create all the callback functions
 
 *Callback functions : there are multiple :
 
     * if the server receive a packet
     * if the server send a packet
     * if the server connects to an access point
     * if the server disconnects from an access point
     ... (you see the idea)
     
     
     
     
     
     
     (not finished)
