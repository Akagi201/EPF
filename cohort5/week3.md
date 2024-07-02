# Week3

## Summary

My main task this week is on based rollup and preconfirmations, and learning revmc and llvm stuffs while doing evm benchmarks

## Attend Meetings

* Attend Chinese EPF meeting.

## Weekly Updates

* Add evm_mlir and revmc to [evm-bench](https://github.com/Akagi201/evm-workshop/tree/master/bench), use same fibonacci contract bytecode, and refined code structure.

```sh
Timer precision: 41 ns
rust_evm                   fastest       │ slowest       │ median        │ mean          │ samples │ iters
├─ bench_evm_mlir          1.915 µs      │ 53.9 ms       │ 1.957 µs      │ 541 µs        │ 100     │ 100
├─ bench_revm_analysed     8.624 µs      │ 1.803 ms      │ 8.832 µs      │ 26.85 µs      │ 100     │ 100
├─ bench_revm_not_analyse  9.29 µs       │ 10.87 µs      │ 9.457 µs      │ 9.472 µs      │ 100     │ 100
├─ bench_revmc             1.583 µs      │ 231.5 µs      │ 1.666 µs      │ 3.996 µs      │ 100     │ 100
╰─ bench_rust_evm          15.87 µs      │ 42.45 µs      │ 16.49 µs      │ 16.71 µs      │ 100     │ 100
```

Look at the fastest result, it's as expected.

* Research on [preconfirmations](https://docs.primev.xyz/)
* Research on [based rollup](https://docs.taiko.xyz/resources/learning-resources/)
