# YangGangCoin
#YangGang street cred. $YGC is a non-monetary ERC20 token to reward supporting Andrew Yang for President.

Learn more at https://medium.com/yang-gang-coin

The Yang Gang Coin token contract address is: 0x87124C52A31587D0D5DBaDaCA6720f249D42856F
https://etherscan.io/token/0x87124C52A31587D0D5DBaDaCA6720f249D42856F

Contract was deployed using Remix:

pragma solidity ^0.5.0;

import "https://github.com/OpenZeppelin/openzeppelin-contracts/blob/master/contracts/token/ERC20/ERC20.sol";
import "https://github.com/OpenZeppelin/openzeppelin-contracts/blob/master/contracts/token/ERC20/ERC20Detailed.sol";

contract YangGangCoin is ERC20, ERC20Detailed {
  uint private INITIAL_SUPPLY = 1000000000e18;
  constructor () public ERC20Detailed("Yang Gang Coin", "YGC", 18)
  {
    _mint(msg.sender, INITIAL_SUPPLY);
  }
  }
