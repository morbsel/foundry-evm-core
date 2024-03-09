### Includes
Foundry EVM core and its necessary dependencies

### Use Cases
- `SharedBackend` in combination with revm

## :warning: **Dependency Configuration (crucial)**

To ensure compatibility and proper functioning of the project, specific versions of `revm-interpreter` and `revm-precompile` must be aligned with `revm-primitives@2.1.0`. This alignment is crucial for maintaining consistent behavior across the dependency graph.

Include the following lines in your project's `Cargo.toml` under `[patch.crates-io]` to set the required versions:

```toml
[patch.crates-io]
revm-interpreter = { git = "https://github.com/bluealloy/revm.git", rev = "76e7c88de07221e1ffe68e05f2be384ff6bcad31" } # Aligns revm-primitives to version 2.1.0
revm-precompile = { git = "https://github.com/bluealloy/revm.git", rev = "76e7c88de07221e1ffe68e05f2be384ff6bcad31" } # Aligns revm-primitives to version 2.1.0 
```


