## Code Used : Solidity + Foundry

```bash

contract DeployScript is Script {
    function setUp() public {}

    function run() public {
        vm.startBroadcast();
        ZkThon z = ZkThon(0x3aC587078b344a3d27e56632dFf236F1Aff04D56);
        z.submitUsername("Timidan");
    }
}

interface ZkThon {
    // Get function
    function getCurrentSubmission() external view returns (string memory);

    // Set function
    function submitUsername(string memory _username) external;
}
```





## Transaction hash

https://explorer.public.zkevm-test.net/tx/0xc0dc618db24af16a8154a6151c508846b76f9ed3f97b88d5c1f3576a936e28a9
