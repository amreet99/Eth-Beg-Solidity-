# Project Title
## Solidity Begineer Assessment

# Description 
This simple contract is written in solidity for developing a smart contract on the Ethereum blockchain. Here the mint and burn function is executed to add and destroy the token and update it into the total supply and the balance.

# Execution 
 Run this program using remix IDE, an online solidity IDE.
 https://remix.ethereum.org/

after opening the IDE create a new workspace and start coding

copy and paste the code :

// SPDX-License-Identifier: MIT
pragma solidity 0.8.18;
/*
       
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






Click on compile on the left. remember to make the compiler to 0.8.18  After compiling now deploy the code by clicking on deploy and run transaction. AAfter that click on the name and symbol it will show the name and symbol as we assigned and check the total supply which is 0 initially. Mint some tokens burn some tokens and check the balance after that you will get the updated token values.

 
# Author
Amrit Paudel
Crafter





