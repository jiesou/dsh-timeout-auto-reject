# dsh-timeout-auto-reject

[简体中文](README.md)

Auto-reject unanswered permission requests.

Any permission request left unanswered for 180s is automatically rejected (fail-closed), and a model-visible `SYSTEM` notice is injected into the agent, which then continues automatically.

Stop being lulled by auto-mode's illusion of safety. When a permission lands on "ask" and you're off-screen, this plugin rejects it by default. Fail-closed is the real safety.

## Install

From npm (prebuilt, recommended):

```sh
dsh plugin --profile web add @jiesou/dsh-timeout-auto-reject
```

Or from GitHub:

```sh
dsh plugin --profile web add github:jiesou/dsh-timeout-auto-reject
```

## After installing

No configuration needed.

The implementation is very simple and compact; feel free to edit `src/index.ts`.

## License

[MIT](LICENSE)