# TimeHolderInterface

Source file [../../contracts/TimeHolderInterface.sol](../../contracts/TimeHolderInterface.sol).

<br />

<hr />

```javascript
pragma solidity ^0.4.8;

import {ERC20Interface as Asset} from "./ERC20Interface.sol";

// BK Ok - Interface for TimeHolder contract
contract TimeHolderInterface {

    mapping(address => uint) public shares;
    mapping(uint => address)  public shareholders;
    mapping(address => uint)  public shareholdersId;
    uint public shareholdersCount = 1;
    uint public totalShares;
    // ERC20 token that acts as shares.
    Asset public sharesContract;
    function totalSupply() constant returns(uint);

}



```