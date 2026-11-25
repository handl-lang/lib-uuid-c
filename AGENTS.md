# lib-uuid-c

Native UUID implementation (C) for the `uuid` port — over the
`rand-c` entropy backend. Pure `.hnl`.

## Layout

| path | role |
| --- | --- |
| `src/index.hnl` | the backend implementation |
| `pkg.hnl` | manifest — `modules: ["uuid-c"]`, dep `rand-c` |
| `scripts/hnl-gate.sh`, `workflows/gate.yaml` | the gate / bupha entry |

## Contract

- Implements the `uuid` contract (`lib-uuid`) natively over C/random
  sources via `rand-c`.

## Verification

```bash
HNL=../host-cli/target/debug/hnl scripts/hnl-gate.sh
```

## License

MIT.

<!-- myco:agent-awareness -->

## Agent awareness

- Session start / any work discussion: run `myco status --prompt`
  before proposing next steps — know the board first.
- User describes new work → offer to capture it (`myco todo add`,
  `issue new`, `proposal new`). Don't wait to be asked.
- Picking up a task: `myco resume <ID>` is the briefing.
- Wrapping up: `myco handoff <ID>` anything resumable; keep statuses
  honest (claimed → in-progress → blocked/done).

<!-- /myco:agent-awareness -->
