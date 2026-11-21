# `stly`: the agentic CLI for Structly

Query and manage your Structly catalog from your terminal or coding agent.

- Discover commands with `stly cli search` and inspect their inputs with `stly schema`.
- Work with structured JSON input and output.
- Preview requests with `--dry-run` before making changes.

Install on macOS with Homebrew:

```sh
brew install --cask structly-io/stly/stly
```

Homebrew automatically registers the tap. The full Cask name approves this tap
for the initial install on Homebrew 7.
After installation, use the short name to update:


```sh
brew update
brew upgrade --cask stly
```

Running `stly` without arguments in an interactive terminal checks for a new
public release, at most once per day. If an update is available, choose **Update
now**, **Skip**, or **Skip until next version** with the arrow keys and Enter
(or press 1, 2, or 3). Escape skips the prompt. Homebrew installations run
`brew upgrade --cask stly`; run `stly` again after Homebrew finishes. Manual
installations receive a download link. Set `STLY_NO_UPDATE_CHECK=1` to disable
checks. Commands with arguments, pipes, and CI runs never check for updates.

Previously registered the tap with the `structly-io/stly.git` URL?
[Switch your existing tap](https://github.com/structly-io/homebrew-stly#switch-an-existing-tap) once.

Sign in and explore your catalog:

```sh
stly auth login
stly apis list --fields id,name
stly --help
stly apis --help
stly apis list --help
```

Run `stly` for a short getting-started guide. Use `stly cli search "find an API"` to
find a command and `stly schema apis list` to inspect its JSON schema. CLI-authored
help, guidance, and errors are in English; server responses and user data retain
their original content.

Supports Apple Silicon and Intel Macs. See the [installation guide](https://docs.structly.io/en/stly/install/)
for setup and updates, or download binaries from [Releases](https://github.com/structly-io/stly/releases).
