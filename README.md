# Forge IDE

A static mockup of the ScrollForge IDE: title bar, activity bar, file Explorer, editor tabs, a "New Files Updated" banner, a code panel, a bottom Problems/Output panel, and a status bar.

## Requirements

- A modern web browser (Chrome, Firefox, Safari, or Edge).
- Git, if you want to clone or update the repository.

No build step, server, or package install is needed.

## Run it

1. Clone the repository:
   ```bash
   git clone https://github.com/askforkris90/forge-ide.git
   cd forge-ide
   ```
2. Open `index.html` in your browser:
   - macOS: `open index.html`
   - Linux: `xdg-open index.html`
   - Windows: `start index.html`

   Or drag the file into an open browser window.

## Use it

- Click a file under **App** in the Explorer to show it in the code panel. `ForgeFetch.ts` shows the original colored code. The other files show plain text.
- Click a tab (`ForgeConfig.ts` or `ScrollForge.ts`) to switch to that file.
- The selected file or tab is highlighted.

## Edit it

Everything is in `index.html`:

- **Styles:** the `<style>` block at the top. Colors are CSS variables in `:root`.
- **Explorer and tabs:** the `.tree` and `.tabs` sections in the body.
- **File contents:** the `files` object in the `<script>` block at the end. Add an entry there and add a matching `data-file` node in the Explorer.

## Commit and push changes

```bash
git add index.html README.md
git commit -m "Describe your change"
git push
```

Set your identity once if git doesn't have one:

```bash
git config --global user.name "Your Name"
git config --global user.email "you@example.com"
```
