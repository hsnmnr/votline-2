# votline-2

Votline is an open source python application, for online voting.

Votline AKA Vote Online consists of 4 Provencial servers Punjab, Sindh, KPK and Balochistan, with each server divided in 2 sub-servers called Part Servers (representing lower and upper parts of province) and one Federal server that connects to all provincial servers. For information sharing between servers and client-server Socket Programming is used with TCP protocol. And Vote Data is saved Json Format.

The structure of application is as follows:

1- Voter add vote info that sent to Provincial Sub Server called Part Server (lower or upper).

2- Part Server saves vote info at "./files/part.json" and Communicate the it to its Provincial Server.

3- Provincial saves vote info at "./files/part.json" and Communicate the it to Fedral Server.

4- Federal server saves vote info at "./files/part.json".

Note:- Each level send successfull message to its caller as it gets the complete vote info.
