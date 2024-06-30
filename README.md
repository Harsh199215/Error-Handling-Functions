# Error-Handling-Functions
This repository deals with 3 inbuilt error handling functions in solidity , For easy understanding I have merged the concept of error handling 
with functions (test1,test2,test3 respectively).

## Prerequisites 

1. Remix ide and how to use it
2. Basic knowledge of Solidity

## Code and explanation

1. "require" is an error handling functions in solidity which takes 2 parameters , first for boolean condition and second for string
messages. 
   
```
 function test1(uint256 _x) public pure returns (uint256) {
        require(_x > 20, "x must be even");
        _x += 10;
        return _x;
    }
```
2. Unlike "require" , "revert" do not require any boolean condition rather it takes only string inputs for messages , but for the boolean part
   we need to use conditional statements like "if".
```
 function test2(uint256 _y) public pure {
        if (_y <= 20) {
            revert("More than 20");
        }
```

3. Assert is little bit different from other two cause it accounts for internal errors rather than input validations and other stuff.
```
    function test3(uint256 _z) public pure returns(string memory){
        assert(_z>20);
        return "All good";
    }
```
## Implementation and Execution 

1. Browse to Remix ide
2. Write up the code
3. Compile and deploy
4. There you go all done!!

## About me

Hi , My name is Harsh <br />
Currently BE-CSE Student at Chandigarh University <br />
Follow me on [twitter](https://x.com/anharsh100k).



  
        
