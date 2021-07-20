# Example Solang

- Tests:
```sh
cd contracts
docker run --rm -it -v $(pwd):/sources hyperledgerlabs/solang -v -o /sources  --target substrate /sources/UniswapV2Router01.sol
```
- Logs:
```
info: Solang version v0.1.7-164-gf29d3f1
thread 'main' panicked at 'expr should not be in cfg: InternalFunctionCall { loc: Loc(0, 7327, 7381), returns: [Address(false)], function: InternalFunction { loc: Loc(0, 7327, 7381), ty: InternalFunction { mutability: Some(Pure(Loc(3, 791, 795))), params: [Address(false), Address(false), Address(false)], returns: [Address(false)] }, function_no: 43, signature: None }, args: [StorageLoad(Loc(0, 7352, 7359), Address(false), StorageVariable(Loc(0, 7352, 7359), StorageRef(true, Address(false)), 0, 0)), Variable(Loc(0, 7361, 7367), Address(false), 169), Load(Loc(0, 7369, 7380), Address(false), Subscript(Loc(0, 7369, 7380), Array(Address(false), [None]), Variable(Loc(0, 7369, 7373), Array(Address(false), [None]), 165), Add(Loc(0, 7376, 7377), Uint(256), Variable(Loc(0, 7374, 7375), Uint(256), 167), NumberLiteral(Loc(0, 7378, 7379), Uint(256), 2))))] }', src/codegen/constant_folding.rs:1065:14
note: run with `RUST_BACKTRACE=1` environment variable to display a backtrace
```
