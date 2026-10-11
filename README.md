# Code with Codespaces

A small, browser-based practice project for learning how to open, customize, and use GitHub Codespaces.

## Project goals

- Create and start a Codespace for this repository.
- Customize the cloud development environment with a `.devcontainer` configuration.
- Edit and run a small example application in the Codespace.
- Commit and push work back to GitHub.

## Quick start

1. Open this repository on GitHub.
2. Select **Code → Codespaces → Create codespace on main**.
3. Wait for the browser-based VS Code environment to finish building.
4. Open a terminal and run:

   ```bash
   python3 --version
   python3 -m http.server 8000
   ```

5. Open the **Ports** tab in the Codespaces interface. If port 8000 is not listed, forward port 8000. Open the forwarded URL to view the project.
6. Edit `index.html`, save, and refresh the browser tab to see your change.

The devcontainer configuration installs Python 3 and provides a consistent VS Code setup. No API keys or external services are required.

## Customize the Codespace

The `.devcontainer/devcontainer.json` file configures the development container, extensions, and forwarding for port 8000. Try changing the project text or colors in `index.html`, then save and preview it.

## Save your work

From the Codespaces terminal:

```bash
git status
git add .
git commit -m "Customize Codespaces practice page"
git push
```

GitHub may ask you to configure a Git author name and email if they are not already set. Use your own preferred Git identity.

## Challenge completion checklist

- [ ] Created and opened a Codespace from this repository.
- [ ] Let the devcontainer build successfully.
- [ ] Ran the example in a browser using forwarded port 8000.
- [ ] Made and saved a code change.
- [ ] Committed and pushed the change to GitHub.
- [ ] Captured a genuine screenshot of the Codespace and working preview.

## Files

- `index.html` — simple practice page to edit and run.
- `.devcontainer/devcontainer.json` — Codespaces environment configuration.

## Troubleshooting

- If the container has not finished building, wait for the build to complete before running commands.
- If Python is unavailable, confirm the devcontainer build completed and reopen the terminal.
- If the preview does not open, verify port 8000 is forwarded and open the URL shown in the Ports tab.
- If `git push` is rejected, run `git status` and follow GitHub's prompt or check whether branch rules require a pull request.
