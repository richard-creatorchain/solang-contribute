# Example Solang

- Tests:
```sh
cd contracts
docker run --rm -it -v $(pwd):/sources hyperledgerlabs/solang -v -o /sources  --target substrate /sources/UniswapV2Router02.sol
```

- Logs (Build success):
```
info: Solang version v0.1.7-168-g087c3e4
/sources/UniswapV2Router02.sol:1:8-23: debug: pragma ‘solidity’ is ignored
/sources/uniswap/lib/contracts/libraries/TransferHelper.sol:1:8-24: debug: pragma ‘solidity’ is ignored
/sources/uniswap/lib/contracts/libraries/TransferHelper.sol:4:1-24: debug: found library ‘TransferHelper’
/sources/uniswap/v2-core/contracts/interfaces/IUniswapV2Factory.sol:1:8-24: debug: pragma ‘solidity’ is ignored
/sources/uniswap/v2-core/contracts/interfaces/IUniswapV2Factory.sol:3:1-29: debug: found interface ‘IUniswapV2Factory’
/sources/interfaces/IUniswapV2Router02.sol:1:8-24: debug: pragma ‘solidity’ is ignored
/sources/interfaces/IUniswapV2Router01.sol:1:8-24: debug: pragma ‘solidity’ is ignored
/sources/interfaces/IUniswapV2Router01.sol:3:1-30: debug: found interface ‘IUniswapV2Router01’
/sources/interfaces/IUniswapV2Router02.sol:5:1-51: debug: found interface ‘IUniswapV2Router02’
/sources/libraries/UniswapV2Library.sol:1:8-24: debug: pragma ‘solidity’ is ignored
/sources/uniswap/v2-core/contracts/interfaces/IUniswapV2Pair.sol:1:8-24: debug: pragma ‘solidity’ is ignored
/sources/uniswap/v2-core/contracts/interfaces/IUniswapV2Pair.sol:3:1-26: debug: found interface ‘IUniswapV2Pair’
/sources/libraries/SafeMath.sol:1:8-23: debug: pragma ‘solidity’ is ignored
/sources/libraries/SafeMath.sol:5:1-18: debug: found library ‘SafeMath’
/sources/libraries/UniswapV2Library.sol:7:1-26: debug: found library ‘UniswapV2Library’
/sources/libraries/UniswapV2Library.sol:66:19-20: warning: local variable 'i' has never been assigned a value, but has been read
/sources/interfaces/IERC20.sol:1:8-24: debug: pragma ‘solidity’ is ignored
/sources/interfaces/IERC20.sol:3:1-18: debug: found interface ‘IERC20’
/sources/interfaces/IWETH.sol:1:8-24: debug: pragma ‘solidity’ is ignored
/sources/interfaces/IWETH.sol:3:1-17: debug: found interface ‘IWETH’
/sources/UniswapV2Router02.sol:13:1-49: debug: found contract ‘UniswapV2Router02’
/sources/UniswapV2Router02.sol:24:50-56: warning: ‘public’: visibility for constructors is ignored
/sources/UniswapV2Router02.sol:70:14-22: warning: function parameter 'deadline' has never been read
/sources/UniswapV2Router02.sol:84:14-22: warning: function parameter 'deadline' has never been read
/sources/UniswapV2Router02.sol:111:14-22: warning: function parameter 'deadline' has never been read
/sources/UniswapV2Router02.sol:214:19-20: warning: local variable 'i' has never been assigned a value, but has been read
/sources/UniswapV2Router02.sol:230:14-22: warning: function parameter 'deadline' has never been read
/sources/UniswapV2Router02.sol:244:14-22: warning: function parameter 'deadline' has never been read
/sources/UniswapV2Router02.sol:253:97-105: warning: function parameter 'deadline' has never been read
/sources/UniswapV2Router02.sol:268:112-120: warning: function parameter 'deadline' has never been read
/sources/UniswapV2Router02.sol:285:112-120: warning: function parameter 'deadline' has never been read
/sources/UniswapV2Router02.sol:302:94-102: warning: function parameter 'deadline' has never been read
/sources/UniswapV2Router02.sol:323:19-20: warning: local variable 'i' has never been assigned a value, but has been read
/sources/UniswapV2Router02.sol:345:14-22: warning: function parameter 'deadline' has never been read
/sources/UniswapV2Router02.sol:361:14-22: warning: function parameter 'deadline' has never been read
/sources/UniswapV2Router02.sol:385:14-22: warning: function parameter 'deadline' has never been read
/sources/uniswap/v2-core/contracts/interfaces/IUniswapV2Factory.sol:4:11-22: warning: event 'PairCreated' has never been emitted
/sources/uniswap/v2-core/contracts/interfaces/IUniswapV2Pair.sol:4:11-19: warning: event 'Approval' has never been emitted
/sources/uniswap/v2-core/contracts/interfaces/IUniswapV2Pair.sol:5:11-19: warning: event 'Transfer' has never been emitted
/sources/uniswap/v2-core/contracts/interfaces/IUniswapV2Pair.sol:24:11-15: warning: event 'Mint' has never been emitted
/sources/uniswap/v2-core/contracts/interfaces/IUniswapV2Pair.sol:25:11-15: warning: event 'Burn' has never been emitted
/sources/uniswap/v2-core/contracts/interfaces/IUniswapV2Pair.sol:26:11-15: warning: event 'Swap' has never been emitted
/sources/uniswap/v2-core/contracts/interfaces/IUniswapV2Pair.sol:34:11-15: warning: event 'Sync' has never been emitted
/sources/interfaces/IERC20.sol:4:11-19: warning: event 'Approval' has never been emitted
/sources/interfaces/IERC20.sol:5:11-19: warning: event 'Transfer' has never been emitted
info: Generating LLVM IR for contract UniswapV2Router02 with target Substrate
info: Saving binary /sources/UniswapV2Router02.wasm for contract UniswapV2Router02
info: Generating Substrate ABI for contract UniswapV2Router02
info: Saving ABI /sources/UniswapV2Router02.contract for contract UniswapV2Router02
```
