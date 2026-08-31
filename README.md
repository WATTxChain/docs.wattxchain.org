# WATTx documentation

Live at **https://docs.wattxchain.org**

`index.html` is a single self-contained page — no build step, no external CSS or JS.
Edit it, commit, push to `main`; GitHub Pages serves it within a minute.

The [whitepaper](https://wattxchain.org/whitepaper.html) is the design rationale;
this is the operator manual: running a node, X25X mining, AuxPoW merged mining,
staking and delegation, the EVM and its AAL quirks, ordinals, privacy, and the
full RPC reference.

Network parameters were read from `src/kernel/chainparams.cpp` on the mainnet
build and confirmed against a live node — not copied from older material.

## DNS

`docs.wattxchain.org` must be a CNAME to `wattxchain.github.io`.
The zone is at IONOS (ui-dns), not Cloudflare. GitHub Pages issues the TLS
certificate itself once that record resolves — the same way `secret.wattxchain.org`
works.
