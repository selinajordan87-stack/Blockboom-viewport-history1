# BLOCKBOOM iPhone historical comparison

Isolated static snapshots, published only in this dedicated test repository.

- Test A: early v0.1, `6946d9f1a78d56a2b1360ddfe9df0a255cadf5c8`.
- Test B: main snapshot, `abd4d3742fd5b9dc9cccf8380403499ce6447a5b`.
- Layout, viewport meta, gameplay and rendering remain from each snapshot.
- Only build base paths, document titles, save keys and manifest scope differ.
- Separate storage prefixes: `blockboom.history-comparison.a.` and `.b.`.
- Neither build reads or overwrites live game saves. No service workers.
- These builds are not yet verified on a real iPhone.

Reproduce from the original Blockboom- repository's branch
`codex/blockboom-history-comparison` with:

`node scripts/build-history-comparison.mjs /absolute/output/path /Blockboom-viewport-history1/`

Pages serves `main`, root directory. No production Blockboom- configuration is changed.
