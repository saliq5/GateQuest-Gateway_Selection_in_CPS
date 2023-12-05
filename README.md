This is a project on Gateway Selection in Cyber Physical Systems using Game Theory done as a part of my course project during 5th Semester. In a CPS, there are devices of multiple wireless technologies hence they cannot directly communicate with each other considering the cost, connectivity and privacy issues. Hence to make this co-existence possible, gateways are used which act as hubs and connect either the devices with same technologies or different technologies as well, due to which gateway distribution problem becomes significant. My aim was to solve the gateway selection problem in a CPS by formulating the situation as a combination of a non cooperative game (lack of controller) and a cooperative game! We model the gateway selection problem as a noncooperative game with players competing for bandwidth of a gateway, analyse the migration trend where we point out at which situation the clients will change their current gateway to increase total benefit of their kind and when they will keep their gateway the same and also analyze the convergence situation at the desired Nash Equilibrium in pure strategies. <br />

<b>Game Modelling</b>: <br />
Consider the devices in the area as players.
These players compete with each other for limited resources where each player can get only one resource which is a gateway.
THE TWIST: Devices of same type can benefit by forming a coalition i.e. by playing a cooperative game as they can share the data within themselves, as a result gain more bandwidth, but at the same time players of a different type compete with the other types using SELFISH ROUTING in order to maximize their payoffs/bandwidth. So we have a COOPERATIVE + NON COOPERATIVE  game in our hand. Can we club the problem into one type?
Yes! Consider all players of type A as Client A and all players of type B as client B.
Now we have two players where each one of them has a strategy to choose between either of the gateways available to them in their radius.
We model this gateway selection problem as a noncooperative game, in which clients select gateways in distributed manner to increase their total bandwidth of their kind.
Now we have a simple NON COOPERATIVE GAME in our hands.

<b>System Design</b>: <br />
1. Network Model: Gateways set G={g1,g2,...,gk}Devices set differentiated by different wireless technologies A={a1,a2,...an}  and B={b1,b2,...bn}. <br />
2. Bandwidth Allocation Model: Each gateway has a total bandwidth of W. The gateway's bandwidth  assigned to each client is wa,I = wb,I =(w/ni+mi)where ni=Number of players of client A connected to the gateway, mi=Number of players of client B connected to the gateway. <br />
3. Gateway Selection Game: It is based on the fact that clients want to maximise their bandwidth (Selfish Routing). If a device increases its benefit, then all devices of its type will have a benefit. A device may change its associated gateway if and only if this migration increases the total bandwidth of its client i.e. new payoff> old payoff. <br />

Base Paper: https://cyberleninka.org/article/n/1430498.pdf





