# tunnel.pizza 🍕

**A public URL for what's running on your machine.** A port, a shell, a coding
agent, a container: one command, no account, no daemon.

```sh
npx tunneld :3000
```

A port is the least of it.

### Interactive shells

```sh
npx tunneld zsh
```

Executes `zsh` on your local machine and makes it accessible in a browser
anywhere in the world.

### Local ports

```sh
npx tunneld :3000
```

Forwards port `3000` on your local machine to a public hostname, so whatever is
listening there is reachable from anywhere.

### Coding agents

```sh
npx tunneld 'claude --resume'
```

Runs `claude --resume` on your local machine and puts the session in a browser,
so you can keep working with it from your phone or another computer. Any agent
that runs in a terminal works the same: Codex, OpenCode, Gemini CLI.

### Multiple ports

```sh
npx tunneld :3000 :4000
```

Forwards ports `3000` and `4000` at once and opens them side by side in one
browser window, two apps on one hostname.

### Code editors

```sh
npx tunneld nvim
```

Runs `nvim` on your local machine in a browser tab, your config and plugins
included.

### Agentic workspaces

```sh
npx tunneld :3000 "next dev" "claude"
```

Starts `next dev`, forwards port `3000` to a public hostname, and opens a
`claude` session beside it: an app, its dev server and an agent, all reachable
from anywhere.

---

- [tunnel.pizza](https://tunnel.pizza) — the site. Sign in with GitHub to
  manage your tunnels; [status](https://tunnel.pizza/status) is public.
- [tunneld](https://github.com/tunnel-pizza/tunneld) — the CLI, in Go.

Made with ❤️ by [Scaffoldly](https://github.com/scaffoldly).
