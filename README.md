HomeAutomation
==============

This is a project to keep myself occupied in a productive way... (And an excuse to do some EE work)

The idea is to have a REST service somewhere on the internet that I can talk to through a client running on Emberjs. When I trigger a command on the client the REST service will forward the command onto wheatever node in the house that action is tied to. These nodes will most likely be Raspberry Pi computers. (Need to have a way to register nodes with the REST service) Each of these nodes will branch out to multiple switch boxes (basically a power strip [1..3 outlets] that is switchable).

REST Service (API)
----
 - Multiple users
   - can own and provide access to nodes/switches
 - Nodes
 - Switches
   - Ability to set intervals
 - rooms
 - views
 - houses?

Client
---
 The client basically just needs to be an interface to interact with all aspects of the API. This will include registering nodes, switches, etc. As well as definining permissions.

Nodes
---
 Nodes are basically just computers that the API talks to in order to interact with the house. This is the start of the physical interaction with the system. (the nodes directly control the relays in the switches)
