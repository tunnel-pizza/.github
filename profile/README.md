# tunnel.pizza 🍕

**Your machine, by the slice.** A public URL for what's running on it: a port,
a shell, a coding agent, a container, or the whole dev box. One command, no
account.

```sh
npx tunneld
```

Your shell, in any browser. <kbd>Ctrl</kbd>+<kbd>K</kbd> then <kbd>q</kbd> puts
it on your phone. Anyone with the address can type into it, so send it like a
password. A port is the least of it.

### Interactive shells

```sh
npx tunneld
```

Shares your `$SHELL` as a terminal in a browser tab, reachable from anywhere.
Nothing else to start, so it is the one to try first.

### Local ports

```sh
npx tunneld :3000
```

Forwards port `3000` on your local machine to a public hostname. Start your app
first: the address serves whatever is listening there.

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
browser window, two apps on one hostname. Start both first.

### Code editors

```sh
npx tunneld nvim
```

Runs `nvim` on your local machine in a browser tab, your config and plugins
included.

### Agentic workspaces

```sh
npx tunneld :3000 'npm run dev' claude
```

Starts `npm run dev`, puts the app it serves on the address, and opens a
`claude` session beside it: your app, its dev server and your agent, all on one
URL. Use the port your dev server prints.

### The whole pie

The cloud dev box you already own. Most tunnels stop at a port, and terminal
sharers stop at the terminal; tunneld does both, on one URL.

| | tunneld | [ngrok](https://ngrok.com/docs/share-localhost/quickstart) | [Cloudflare Quick Tunnels](https://developers.cloudflare.com/cloudflare-one/networks/connectors/cloudflare-tunnel/do-more-with-tunnels/trycloudflare/) | [Tailscale Funnel](https://tailscale.com/kb/1223/funnel) | [VS Code tunnels](https://code.visualstudio.com/docs/remote/tunnels) | [sshx](https://sshx.io/) |
| --- | :-: | :-: | :-: | :-: | :-: | :-: |
| No account to sign up for | ✅ | – | ✅ | – | – | ✅ |
| A local port on a public URL | ✅ | ✅ | ✅ | ✅ | ✅ | – |
| A shell or agent in a browser tab, for anyone with the link | ✅ | – | – | – | – | ✅ |
| Everyone with the link types into the same session | ✅ | – | – | – | – | ✅ |
| An app and a terminal on one URL, with no config | ✅ | – | – | – | – | – |

<sub>From each tool's own documentation, September 2026. A tool that needs
another account or hand-built config to do a thing counts as not doing it.
Anyone with a tunnel's address reaches what's behind it, so send it like a
password.</sub>

---

- [tunnel.pizza](https://tunnel.pizza) — the site. Sign in with GitHub to
  manage your tunnels; [status](https://tunnel.pizza/status) is public.
- [tunneld](https://github.com/tunnel-pizza/tunneld) — the CLI, in Go.

Made with ❤️ by [Scaffoldly](https://github.com/scaffoldly).
