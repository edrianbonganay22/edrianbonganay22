- 👋 Hi, I’m @edrianbonganay22
- 👀 I’m interested in ...
- 🌱 I’m currently learning ...
- 💞️ I’m looking to collaborate on ...
- 📫 How to reach me ...

<!---
edrianbonganay22/edrianbonganay22 is a ✨ special ✨ repository because its `README.md` (this file) appears on your GitHub profile.
You can click the Preview link to take a look at your changes.
--->

CREATE A TOKEN

This SOLIDITY assessment aims to create an nft token in a simple and easy way in order for newbie students can understand with ease.

## Description

This contract is a basic simulation on how NFTs work and how to create it.

## Getting Started


### Executing program

- First you need to create string variables.
- Use a function called mapping address and make it public.
- Create a mint function that both parameters has an address and uint.
- Create a burn function, it is nearly the same as the mint function but replace the "+" with a "-" and add a if statement.
- Deploy your NFT and try its features.
```

contract MyToken {

    // public variables here
    string public tokenName = "USCOIN";
    string public tokenAbbrv = "USCN";
    uint public totalSupply = 0;

    // mapping variable here
    mapping (address => uint) public balances;

    // mint function
    function mint (address add, uint val)public {
        totalSupply += val;
        balances[add] += val;
    }

    // burn function
       function burn (address add, uint val)public {
        if (balances[add] >= val){
         totalSupply -= val;
         balances[add] -= val;
        }
    }




}
```

## Authors

Contributors names and contact info

Edrian Bonganay
[Facebook.com/](https://facebook.com/)

