### Packet Logging

* Useful for developers, it can be very handy to see what activitiy is happening realtime. We now have the ability to sink it to any output format simultaneously.

### Packet Categories

```
select * from logsys_categories where log_category_description like '%packet%';
+-----------------+------------------------------------+----------------+-------------+--------------+
| log_category_id | log_category_description           | log_to_console | log_to_file | log_to_gmsay |
+-----------------+------------------------------------+----------------+-------------+--------------+
|               5 | Packet: Client -> Server           |              0 |           0 |            0 |
|              39 | Packet: Server -> Client           |              0 |           0 |            0 |
|              40 | Packet: Client -> Server Unhandled |              0 |           0 |            0 |
|              41 | Packet: Server -> Client With Dump |              0 |           0 |            0 |
|              42 | Packet: Server -> Client With Dump |              0 |           0 |            0 |
+-----------------+------------------------------------+----------------+-------------+--------------+
5 rows in set (0.04 sec)
```

#### Enable in Game (Example)

Below would enable client -> server direction packet logging to the client

```
#logs set gmsay 5 1
```

## Server to Client

All server packets that are sent to the client, the only packet types that aren't sent to the client while in game are the message packets themselves because that would cause a loop


<p align="center">
<img src="/EQEmu/Server/wiki/images/llm7EXY-opt.gif?raw=true">
</p>

## Client to Server

Packets being sent from client to server

<p align="center">
<img src="/EQEmu/Server/wiki/images/8t4tkrB.gif?raw=true">
</p>

## Unhandled Packets

In this example - a client clicking a 'Krono' is unhandled by the server, at which it dumps a packet of data sent from the client

<p align="center">
<img src="/EQEmu/Server/wiki/images/XkPDXb9.gif?raw=true">
</p>

### Packet Logging Levels

*   The main differentiator when deciding how much information you want to see with each packet, you use two different but very smiliar categories for each type. It all comes down to whether or not you want to see the packet dump data with the packet or not. As of this time, Packet: Client -> Server Unhandled always dumps the packet because they are far less frequent.
    *   Packet: Client -> Server
    *   Packet: Server -> Client
    *   Packet: Server -> Client With Dump
    *   Packet: Server -> Client With Dump

## Packet Information (With Dump)

Below is an example of a full packet payload being output to the client

<p align="center">
<img src="/EQEmu/Server/wiki/images/C9SnDRD.gif?raw=true">
</p>