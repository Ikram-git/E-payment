During the development process, the latest python version was used so  to run our system, the latest python version is recommended. It is recommended to run and test the project on one of the following IDEs: VS Code, PyCharm Community Edition, IntelliJ IDEA Ultimate edition. These IDEs are recommended as development and testing was performed using either of these platforms.
To run our system go to file “Node.py” and run it. It is recommended to use port number “3009” or “3008”

To use our system on windows it is recommended to run following commands in terminal in Pycharm: 
1. Creating an account
 $ python console account create 
It will assign a pair of public and private keys along with an address. Refer to the database to view the address and public key of the created account .
2. Mining
 $ python console miner start 3008  
It will start mining at nodes with a port number specified. The port number should be the same as the one used to run the Node.py file. To look for blocks mined, go to the database to see the latest  blockchain.
Mined blockchain/current state of blockchain can be viewed by using following command:
$ python console blockchain list


3. Transactions
 $ python main.py transact transfer sender_address reciever_address amount 
To make a  transaction, create another account and look for addresses of both accounts in database and paste them in above command along with the amount
Transaction list can be viewed on CLI as well:
$ python console tx list


4.  Network
$ cd new directory
$ python console node add 3008 
$ python console node run 3009

Copy the code folder to a different directory and run the above commands assuming that the initial node was running at port 3008. When mining is done on new node(3009) the blocks mined at new node are visible to other nodes using longest chain rule
Note: While running the second command,  if there is an error, that means you are not using the latest version of python or it may not be active.
