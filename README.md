# EtheriumPyramidSample
Solidity smart contract based on pyramid scheme of distribution with comission to owner of contract

Solidity ver 0.2.1.

Sends value of sender transaction with multiply percents if it has proper balance.
There are two rows: senders and payers
Senders update every time it gets transaction
Payers update every time it pays to sender

HOW IT WORKS:
-People send etherium from 0.01 to 0.025
-If people send bigger or smaller transaction, contract give him back this value
-Contract waits for another etherium sender
-If balance is bigger than sended value * 111% - contract sends this value to sender
-If balance is not enough, contract waits for another sender

EXAMPLE:
1* send 0.02 eth
contract* set 1 to pay 0.02*111%
contract* pay owner commission 0.02*005%
2* send 0.012 eth
contract* set 2 to pay 0.012*111%
contract* pay owner commission 0.012*005%
contract* check balance
contract* pay 1 0.02*111%
3* send 0.025 eth
contract* set 3 to pay 0.025*111%
contract* pay owner commission 0.025*005%
contract* check for balance
contract* pay 2 0.012*111%
1* send 0.5 eth
contract* pay owner commission 0.5*005% 
contract* pay 1 0.5 eth - commission ^



