// SPDX-License-Identifier: MIT
pragma solidity ^0.8.0;

contract TechAcademy {
    uint256 public number;
    string public message;

    constructor(uint256 _startingPoint, string memory _startingMessage) {
        number = _startingPoint;
        message = _startingMessage;
    }

    function getNumber() external view returns(uint256) {
        return number;
    }

    function increaseNumber() external {
        number++;
    }

    function decreaseNumber() external {
        number--;
    }

    function setMessage(string memory newMessage) public {
        message = newMessage;
    }
}
