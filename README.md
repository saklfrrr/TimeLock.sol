# TimeLock.sol
TimeLock.sol
pragma solidity ^0.8.20;
contract TimeLock {
    uint public unlockTime;

    constructor(uint _time){
        unlockTime = block.timestamp + _time;
    }
}
