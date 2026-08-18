# dsh-timeout-auto-reject

Auto-reject unanswered permission requests.

[English](README.en.md)

自动拒绝未应答的权限请求。

任何 permission 请求如果在 180s 内无人应答，插件会自动拒绝，同时向 agent 注入一条模型可见的 `SYSTEM` 提示，agent 不停止，自动继续运行。

别再被“auto-mode”的安全感骗了，fail-close 才是真安全

## 安装

从 npm 安装（预构建产物，推荐）：

```sh
dsh plugin --profile web add @jiesou/dsh-timeout-auto-reject
```

或从 GitHub 安装：

```sh
dsh plugin --profile web add github:jiesou/dsh-timeout-auto-reject
```

## 安装之后

无需任何配置。

代码实现非常简单小巧，你可以随意修改 `src/index.ts`

## License

[MIT](LICENSE)
