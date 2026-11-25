# lib-uuid-c

Native UUID implementation (C) for the `uuid` port.

## Layout

```text
src/        the .hnl sources
pkg.hnl     package manifest — modules, deps, description, license
scripts/hnl-gate.sh   the gate
workflows/gate.yaml       bupha entry (handl-gates)
```

## Gate

```bash
HNL=../host-cli/target/debug/hnl scripts/hnl-gate.sh
```

## License

MIT.
