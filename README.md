# lib-uuid-c

Native UUID implementation (C) for the `uuid` port.

Part of the `handl-lang` org split (ADR-0128). History is a `git subtree
split` of `kit-canonical/handl-packages/uuid-c/`.

## Layout

```text
src/        the .hnl sources
pkg.hnl     dependencies, when any: `{ deps: { <name>: "branch:<ref>" } }`
```

Dependencies: see `pkg.hnl`

## Gate

```bash
HNL=../cli/target/debug/hnl scripts/hnl-gate.sh
```
