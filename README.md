# Beba Blockchain Master Node
This node provide services to interact with blockchain, set your configuration, start node and join to the network crypto flow 2021.
This node allow safe communication bethwen your platform`s ane Beba Blockchain, this way you can access to:

A Node to create applications and services with Node JS, it is extensible and configurable to adapt quickly to management and administration platforms.
The Node contains blockchain services, wallet services and cryptocurrency transactions, transaction mining. The node allows to extend its 
capabilities which makes it scalable according to your needs. It is possible to add a backoffice and expose API services for your community.


Services:

- Connect Node
- Make pin blockchain
- Create wallet
- Get wallet info
- Make instant transactions
- Get blockchain public info
- Create Blockchain Users
- Get list Confirmed transactions


#Pre Install
System Windows 10 2 RAM Core i3 (Min) Open PORT Configuration

Install Git
Install Composer
Install Node JS
Install Babel
Install NodeMon
Allow Full Permission to node folder

# Installation
Clone from https://github.com/BebaBlockchain/master_node.git
npm install
Composer Install


Once we have all the components installed on the server, we access the path of our example node via CMD (Command Line):
C:/ruta_al_nodo/MASTER_NODO/

# Starting Node
For the node to start working, we run the command created

YourPath/EXAMPLE/MASTER_NODO>yarn start

***** The console will show the following and the NODE IS READY and working in the Port: 3000 Service
Service HTTP:3000 listening...
Master Node Online on:
https://blockexplorer.club


# Node Services

Once the node is online, we can access the aforementioned services to start processing transactions and requests to the blockchain (BEBA). The services and a brief explanation of their use are listed below.

The first call, after run (yarn start)


1.0 PIN BLOCKCHAIN
This service make pin and start the general service node.
POST http://localhost:3000/pin_blockchain
No Parameters


2.0 MASTER NODE INFO
This service return information of this node configuration
POST http://localhost:3000/master_node
No Parameters


3.0 CREATE REQUEST WALLET
This service request wallet from blockchain and return a user
POST http://localhost:3000/pin_blockchain
No Parameters


4.0 GET WALLET INFO
This service request wallet information
send in parammeters json the wallet than you are lookin for
POST http://localhost:3000/nodo_get_wallet_info
Parameters
{
  "wallet":"CDvVDdf8635t73ue83jh8ud8jdid39EDDEDEDEmjd8837363653icCECECECEE"
}


5.0 GET ALL WALLET
This service request all wallets from node
POST http://localhost:3000/nodo_all_wallets
No Parameters



6.0 SERVICE INSTANT SEND
This service allow instant send crypto coins bethween wallets on blockchain
POST http://localhost:3000/nodo_send
Parameters (String)
{
  "wallet":"CDvVDdf8635t73ue83jh8ud8jdid39EDDEDEDEmjd8837363653icCECECECEE",
  "recipient":"CDvVDdf8635t73ue83jh8ud8jdid39EDDEDEDEmjd8837363653icCECECECEE",
  "amount":"21"
}


7.0 GET BLOCK INFO
This service request info of blocks validated in blockchain
POST http://localhost:3000/nodo_blocks
No Parameters


7.0 GET LAST CONFIRMED TRANSACTIONS
This service return last transactions of wallet
POST http://localhost:3000/nodo_last_transactions
Parameters
{
  "wallet":"CDvVDdf8635t73ue83jh8ud8jdid39EDDEDEDEmjd8837363653icCECECECEE"
}


# License
Code released under the MIT license.

Copyright 2020-2021 Beba Coin, Inc.
