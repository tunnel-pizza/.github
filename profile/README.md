# tunnel.pizza 🍕

**Slice and share your machine.** Put what's running on it on a public URL: a
port, a shell, a coding agent, a container, or your whole workspace. One
command, no account.

```sh
npx tunneld
```

Open your shell in any browser. Share your URL and continue on the go or
collaborate.

### Interactive shells

```sh
npx tunneld
```

Share your `$SHELL` in a browser tab. Nothing else to start, so try this one
first.

### Local ports

```sh
npx tunneld :3000
```

Start your app, then put port `3000` on a public URL.

### Coding agents

```sh
npx tunneld 'claude --resume'
```

Pick your `claude` session back up from your phone or another computer. Swap in
any terminal agent: Codex, OpenCode, Gemini CLI.

### Multiple ports

```sh
npx tunneld :3000 :4000
```

Start both your apps, then open them side by side on one hostname.

### Code editors

```sh
npx tunneld nvim
```

Open `nvim` in a browser tab, with your config and plugins.

### Agentic workspaces

```sh
npx tunneld :3000 'npm run dev' claude
```

Run `npm run dev`, your app and `claude` side by side on one URL. Use the port
your dev server prints.

### The whole pie

Your whole workspace on one URL: your app, your dev server and your agent, with
no account.

| | tunneld | [ngrok](https://ngrok.com/docs/share-localhost/quickstart) | [Cloudflare Quick Tunnels](https://developers.cloudflare.com/cloudflare-one/networks/connectors/cloudflare-tunnel/do-more-with-tunnels/trycloudflare/) | [Tailscale Funnel](https://tailscale.com/kb/1223/funnel) | [VS Code tunnels](https://code.visualstudio.com/docs/remote/tunnels) | [sshx](https://sshx.io/) |
| --- | :-: | :-: | :-: | :-: | :-: | :-: |
| No account to sign up for | ✅ | – | ✅ | – | – | ✅ |
| A local port on a public URL | ✅ | ✅ | ✅ | ✅ | ✅ | – |
| A shell or agent in a browser tab, for anyone with the link | ✅ | – | – | – | – | ✅ |
| Everyone with the link types into the same session | ✅ | – | – | – | – | ✅ |
| An app and a terminal on one URL, with no config | ✅ | – | – | – | – | – |

<sub>Checked against each tool's own docs, September 2026: click a name to read
them. Needing another account or hand-built config counts as a no. Send your
tunnel's address like a password: anyone with it reaches what's behind it.</sub>

---

- [tunnel.pizza](https://tunnel.pizza) — the site. Sign in with GitHub to
  manage your tunnels; [status](https://tunnel.pizza/status) is public.
- [tunneld](https://github.com/tunnel-pizza/tunneld) — the CLI, in Go.

Made with ❤️ by [Scaffoldly](https://github.com/scaffoldly).
