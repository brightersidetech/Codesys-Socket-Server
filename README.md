# Codesys Socket Server
This project Implements a Socket Server in Codesys to communicte with socket clients over TCP. The sever Listens for client connections, accepts connections, reads data and send back responses over TCP. Any client regardless of its implementaion is able to connect to the server, send data and recieve responses


### Requiremets
- To open the Codeys project, you need to have Codeys 3.5.19.5 or Later
- For the Python Socket client, you need to have python 2.7 otr later


### Instructions
PLC Side (Sockey Server)
- Open the Codesys Project
- Modify the ```sIPAddress``` paramter with the correct interface address on which you wish to bind the socket
- Modify the ```wPort``` parameter with the correct port on which you wish your sever to listen for conneections
- Update the Device with the correct controller/ device
- Upload the project, and start the application, then set the ```xStart``` Parameter to True

Python side (Socket client)
- Open the ```socket_client.py``` Script inside the ```Scoket_Client```Folder
- Update the HOST paramter with the correct Socket server address
- Update the PORT Paramter with the Correct Socket server Port 
- Set the desired message to send to the server 
- Run the Script: ```python socket_client.py```