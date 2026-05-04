# MultiBalance.sol
MultiBalance.sol
pragma solidity ^0.8.20;
contract MultiBalance {
    mapping(address => uint) public balance;

    function deposit() public payable {
        balance[msg.sender] += msg.value;
    }
}
