# HashCompare.sol
Remix - Deploy Contract On Base Network HashCompare.sol
// SPDX-License-Identifier: MIT
pragma solidity ^0.8.20;

contract HashCompare {
    function compare(string memory a, string memory b) public pure returns (bool) {
        return keccak256(abi.encodePacked(a)) == keccak256(abi.encodePacked(b));
    }
}
