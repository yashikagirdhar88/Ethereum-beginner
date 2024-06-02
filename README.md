# Ethereum-beginner
-->So the project is to create a Token.
-->>Here, we have our contract as MyToken.
-->>This contract have various public variables such as 
    1. Token Name stores the name of token here token name is "PlayCard" ,
    2. Token Abbrv. stores the abbrevation of token "PlayCard" here it is abbreviated "PC" ,
    3. Total Supply has information about total supply of Token, initially it is set to zero.
    these all basically store details about our coin.
-->After this mapping of Addresses to balances is there as (mapping(address=>uint)public balances;), it associates each address with its token balance and simply track
   how many tokens each address owns.
-->Now we have a mint function having two parameters an address and a value, it allows creating new tokens and assigns them to a specified address.
   _address parameter is the address to which newly minted tokens will be credited and value parameter has the number of tokens to be minted. 
   mint function increases the totalsupply by specified value and also updates the balance of the given address accordingly.
-->Now, in burn function (opposite of mint function) it also have two parameters an address and a value but it destroys Token from specified addresss.
   _address parameter is the address from which tokens will be destroyed or burned and value is the number of token burned. 
    this function have conditionals to check the balance of sender is greater than or equal to the amount that is to be burned and if it is true than it decreases the 
    total supply and the balance of the given address by a specified value.
    -->So basically this contract implements a simple and basic form of token management , illustrating the concept of mint and burn function in blockchain 
