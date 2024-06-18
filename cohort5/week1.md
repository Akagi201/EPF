# Week 1

## Summary

Get familiar with what others are talking about and dong on EL. Researches on High performance EVM implementations.

## Attend Meetings

* Attend Chinese EPF Weekly Meeting.
* Attend EOF Implementers Call [#50](https://github.com/ethereum/pm/issues/1063)

## Weekly Updates

* Read [EOFv1 Spec/EIP-7692](https://github.com/ipsilon/eof/blob/main/spec/eof.md)
* Learning [EPF.wiki EVM section](https://epf.wiki/#/wiki/EL/evm)
* Reading Source code of [rust-ethereum/evm](https://github.com/rust-ethereum/evm)
* Research and reading docs of Monad.
* Research and reviewing code of lambdaclass's [evm_mlir](https://github.com/lambdaclass/evm_mlir) (300% to 600% times higher than revm), [article](https://blog.lambdaclass.com/evm-performance-boosts-with-mlir)
* Get familiar with Nethermind Node, and performance change, up to 1.5 GGas/s, review [v1.27-rc](https://github.com/NethermindEth/nethermind/releases/tag/1.27.0-rc)
* Optimism EIP1559 [gas strategy](https://docs.optimism.io/chain/differences), orderly increasing block gas limit to [100m](https://testnet-explorer.orderly.org/blocks), base chain [90m](https://basescan.org/block/15812947), [orderly gas/s to top 5]
(https://rollup.wtf/), write a [base fee calculator](https://gist.github.com/Akagi201/22b868970e51b1bcc70bd3217c160525)

## EVM Bench

[evm-bench](https://github.com/Akagi201/evm-workshop/blob/master/bench/benches/rust_evm.rs) - benchmark between [rust-evm](https://github.com/rust-ethereum/evm) and [revm](https://github.com/bluealloy/revm)

```sh
rust_evm           fastest       │ slowest       │ median        │ mean          │ samples │ iters
├─ bench_revm      18.54 µs      │ 840.8 µs      │ 19.08 µs      │ 27.51 µs      │ 100     │ 100
╰─ bench_rust_evm  30.66 µs      │ 106.4 µs      │ 32.04 µs      │ 32.87 µs      │ 100     │ 100
```
