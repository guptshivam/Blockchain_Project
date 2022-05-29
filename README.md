# Blockchain_Project
To create a cryptocurrency using python

How to run it---->
First, install requirements.txt.
pip install -r requirements.txt
Then you have 2 options:
Run miner.py to become a node and start mining
Run wallet.py to become a user and send transactions (to send transactions you must run a node, 
in other words, you must run miner.py too)
Important: DO NOT run it in the python IDLE, run it in your console. The miner.py uses parallel 
processing that doesn't work in the python IDLE.

How this code works---->
There are 2 main scripts:
miner.py
wallet.py
Miner.py
This file is probably the most important. Running it will create a node (like a server). From here you 
can connect to the blockchain and process transactions (that other users send) by mining. As a 
reward for this work, you recieve some coins. The more nodes exist, the more secure the 
blockchain gets.
miner.py has 2 processes running in parallel:
The first process takes care of mining, updating new blockchains and finding the proof of work.
The second process runs the flask server where peer nodes and users can connect to ask for the 
entire blockchain or submit new transactions.

Wallet.py
This file is for those who don't want to be nodes but simple users. Running this file allows you to 
generate a new address, send coins and check your transaction history (keep in mind that if you 
are running this in a local server, you will need a "miner" to process your transaction). When 
creating a wallet address, a new file will be generated with all your security credentials. You are 
supposed to keep it safe.

Working----->
  Running miner.py 
    When we ran miner file using command “python miner.py” than it showed
    ![image](https://user-images.githubusercontent.com/91245289/170854621-221bcef2-b32a-4c90-b24e-102e6d5d6674.png)
    
   Initially when there was no any transaction in mempool than minor did not get any 
   transaction to mine.so our program has showed “NO transaction… skipping”.
   
  Running wallet.py
      When we ran wallet.py file than it showed:
      ![image](https://user-images.githubusercontent.com/91245289/170854660-5dbb07ab-0fa9-4f45-9e46-475f65848ccc.png)
      when we entered “1” as input than it asked the name of the user after that we entered name 
      “Shubham” then it created a file named Shubham.txt which contained public key and private 
      key of the user.
      
      ![image](https://user-images.githubusercontent.com/91245289/170854714-26ea55f4-91fc-476e-b16a-e7ee899eea4d.png)
      
   Doing transaction:

     While doing transaction our program demanded public key and private key of the sender and also public key of the receiver wallet. It checked all the keys and did      one transaction.
     ![image](https://user-images.githubusercontent.com/91245289/170854773-2fabc844-9a4c-49d7-b1f6-59c32feb0ccd.png)
     
     This transaction arrived in the mempool and miner mined it and added a block to the blockchain.
     
     ![image](https://user-images.githubusercontent.com/91245289/170854797-a8578763-02db-4b09-acb5-b1f74362a6e5.png)
     
     We can also see in the user transaction:
     
     ![image](https://user-images.githubusercontent.com/91245289/170854802-9d5491df-d9f7-4224-aff3-60236fc8f936.png)
     
Results and Discussion----->

Blockchain provide transparency in the transaction. It is very disruptive technology.in this project 
,we have created a cryptocurrency named NITP coin which is working based on blockchain 
technology implement in python high level programming language. We can also make this project 
more interactive using user interface.







   
    

 
