# Project Title
## solidity Begineer Assessment

# Description 
This simple contract is written in solidity for developing a smart contract on the Ethereum blockchain. Here the mint and burn fucntion is executed to add and destroy the token and update it into the total supply and the balance.

# Execution 
 Run this program using remix IDE, an online solidity IDE.
 https://remix.ethereum.org/

after opening the IDE create a new workspace and start coding

copy and paste the code :

// SPDX-License-Identifier: MIT
pragma solidity 0.8.18;
/*
       REQUIREMENTS
    1. Your contract will have public variables that store the details about your coin (Token Name, Token Abbrv., Total Supply)
    2. Your contract will have a mapping of addresses to balances (address => uint)
    3. You will have a mint function that takes two parameters: an address and a value. 
       The function then increases the total supply by that number and increases the balance 
       of the “sender” address by that amount
    4. Your contract will have a burn function, which works the opposite of the mint function, as it will destroy tokens. 
       It will take an address and value just like the mint functions. It will then deduct the value from the total supply 
       and from the balance of the “sender”.
    5. Lastly, your burn function should have conditionals to make sure the balance of "sender" is greater than or equal 
       to the amount that is supposed to be burned.
*/
contract DemoToken {
    // Public variables
    string public name = "complete";
    string public symbol = "comp";
    uint public totalSupply = 0;

    // Mapping of addresses to balances
    mapping(address => uint) public balances;

    // Mint function
    function mint(address _address, uint _value) public {
        totalSupply += _value;
        balances[_address] += _value;
    }

    // Burn function
    function burn(address _address, uint _value) public {
        require(balances[_address] >= _value, "Insufficient balance to burn");
        totalSupply -= _value;
        balances[_address] -= _value;
    }
}






## click on compile on the left. remember to make the compiler to 0.8.18   
After compile now deploy the code by clicking on deploy and run transaction.
after that click on the name and symbol it will show the name and symbol as we assigned and check the total supply which is 0 initially.
mint some tokens burn some tokens and check the balance after that you will get the updated token values.

 
# Author
## Amrit Paudel
Crafter






