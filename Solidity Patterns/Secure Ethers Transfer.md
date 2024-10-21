## Intent
---
To secure transfer of ether from a contract to another address
***
## Implementation
***
- transfer 
	- 2300 gas stipend
	- throws on failure
	- example ```
	```solidity
	function transferFund() external payable {
		address payable(receiver).transfer(amount);
	}
	```

***
- send 
	- 2300 gas stipend
	- false on failure
	- example
	```solidity
	function transferFund() external payable {
		if (!address payable(receiver).transfer(amount)) 
		{
			//handle error
		}
	}
	```
***
- call (recommend way to use after 2019)
	- gas can be specific
	- false on failure
	- **vulnerable to reentrancy attack if not carefully handle**
```soldity
	function transferFund() external payable {
		(bool success, _) = address payable(receiver).call{value: gas}('');
	}
```

#### Example implementations
- [[MultiSend Contract]]
- Crypto Sprites contract

#### Also
- [[Reentrancy Attacks]]
- [[Fallback functions]]
- [[Checks-Effects-Interactions]]
- [[Guard Check Pattern]]