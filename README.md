IEC60870-5-104
The software implements communication via IEC60870-5-104 to OPC UA on Optix Edge Device Rockwell Automation, you can use multiple instances of "MASTER" and "SLAVE" objects to connect Optix with PLCs or RTU that use this protocol.

In v1.0.1 are supported:
M_SP_NA_1 - Single-point information
M_DP_NA_1 - Double-point information
M_ME_NA_1 - Measured value, normalised value
C_SC_NA_1 - Single command
C_DC_NA_1 - Double command
C_IC_NA_1 - Interrogation Command
M_EI_NA_1 - End of Initialization

By command "setParam(byte,bool)" you can set some telegrams to be sent to the connection establishment:
0 - M_EI_NA_1 - End of Initialization
1 - C_IC_NA_1 - Interrogation Command (Valid only for MASTER instance)

The library was tested on Optix Edge (NodeRed Docker Container) by Ethernet.
For IEC104 - Server - Required : IEC 60870-5-104 Server Simulator
For OPC UA, Module already added in  Json File,

For More  Information check  " Complete_IEC104_OPCUA_SOP.pdf".
