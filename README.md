- 👋 Hi, I’m @edrianbonganay22
- 👀 I’m interested in ...
- 🌱 I’m currently learning ...
- 💞️ I’m looking to collaborate on ...
- 📫 How to reach me ...

<!---
edrianbonganay22/edrianbonganay22 is a ✨ special ✨ repository because its `README.md` (this file) appears on your GitHub profile.
You can click the Preview link to take a look at your changes.
--->

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
