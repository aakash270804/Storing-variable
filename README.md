# Storing-variable
This Solidity contract allows users to store and retrieve four different types of variables: an integer (uint), a string, a boolean, and an Ethereum address. The contract provides functions to set and get the values for each of these variables.

## Description
The VariableStorage contract is a simple example of how to store different types of data in a Solidity smart contract. The contract has four public variables:

number: an unsigned integer
text: a string
flag: a boolean
userAddress: an Ethereum address
Users can interact with the contract through the provided functions to set or retrieve the values of these variables.

## Getting Started
### Installing
To use this contract, you can compile and deploy it using an Ethereum development environment like Remix.

Open the Remix IDE.
Create a new file with a .sol extension (e.g., VariableStorage.sol).
Copy and paste the following code into the file:

    
    // SPDX-License-Identifier: MIT
    pragma solidity 0.8.26;\
    contract VariableStorage {
    
    // Declare four variables
    uint public number;
    string public text;
    bool public flag;
    address public userAddress;

    function setNumber(uint _number) public returns (uint) {
        number = _number;
        return number;
    }

    function getNumber() public view returns (uint) {
        return number;
    }

    function setText(string memory _text) public returns (string memory) {
        text = _text;
        return text;
    }

    function getText() public view returns (string memory) {
        return text;
    }

    function setFlag(bool _flag) public returns (bool) {
        flag = _flag;
        return flag;
    }

    function getFlag() public view returns (bool) {
        return flag;
    }

    function setUserAddress(address _userAddress) public returns (address) {
        userAddress = _userAddress;
        return userAddress;
    }

    function getUserAddress() public view returns (address) {
        return userAddress;
    }
    }

### Executing Program
Compile the contract using the Solidity compiler in Remix. Ensure the compiler version is set to 0.8.26.

Deploy the contract using the "Deploy & Run Transactions" tab.

After deploying, you can use the following functions to set and get values:

setNumber(uint _number) and getNumber(): Sets and retrieves the number.
setText(string memory _text) and getText(): Sets and retrieves the text.
setFlag(bool _flag) and getFlag(): Sets and retrieves the flag.
setUserAddress(address _userAddress) and getUserAddress(): Sets and retrieves the userAddress.

## Help
Ensure that:

You are using the correct data types when setting values (e.g., a valid uint for number, string for text).
Use the correct Solidity version (0.8.26) for compatibility.

## Authors

Aakash Raj
akashraj2708@gmail.com

##License
This project is licensed under the MIT License - see the LICENSE.md file for details.
