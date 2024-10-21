- Contracts and [[Technical Terms#^EOA| EOA]] **can not prevent** someone sending them ethers.
- Contracts can react to **regular transfer** with fallback functions.
- Contracts can not react to receiving Ethers in two ways
	- One way is "mine to" the contract address
	- Second is via `selfdestruct(targetAddress)`.

#### Also
- [[Mining]]