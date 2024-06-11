// SPDX-License-Identifier: MIT
pragma solidity >=0.6.12 <0.9.0;

contract myproject {
  
  string public T_name = "def_name";
  string public T_address = "def_address";
  uint public Total = 0;
  
  mapping(address => uint) public my_balances;

  function mint_token (address myadd, uint new_val) public {
    Total += new_val;
    my_balances[myadd] += new_val;
  }

  function burn_token (address myadd, uint new_val) public {
    if(my_balances[myadd] >= new_val){
      Total -= new_val;
      my_balances[myadd] -= new_val;
    }
  }
}
