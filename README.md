# libsnark Rust wrapper
Simple wrapper for libsnark library.

## Introduction 

!! NOTE THIS IS A WIP, please help if you have cycles,
This is a dependency for `XaeroID` so wait until its 1.0 before using 
it in prod, our timeline is ready for prime time by July 15 !!

## Usage
Here's how it `would` look once ready:

```rust

    use libsnark_rs::{prove_role, verify_role};
    
    let proof = prove_role("keys/role.pk", 7, 5);
    assert!(verify_role("keys/role.vk", 5, &proof));

```