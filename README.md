# Example Solang

- Tests:
```sh
cd contracts
docker run --rm -it -v $(pwd):/sources hyperledgerlabs/solang -v -o /sources  --target substrate /sources/UniswapV2Router01.sol
```
- Logs:
```
info: Solang version v0.1.7-157-ge64a7a2
/sources/UniswapV2Router01.sol:12:30-38: error: unrecognised token `override', expected ";", "="
/sources/UniswapV2Router01.sol: error: no valid contracts found
```