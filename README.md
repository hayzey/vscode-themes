# vscode-themes
A little collection of my VS Code themes. 👩‍💻

## Development

Contributors: feel free to open an issue or a PR with any fixes. The following is for my own future reference...

### Publishing an update

See the [VS Code docs about publishing an extension](https://code.visualstudio.com/api/working-with-extensions/publishing-extension). You need to **package**, then **publish** the extension after making changes. There are some scripts for this.

First, you need `vsce` installed (CLI for building/publishing VS Code extensions): `npm install -g @vscode/vsce`

1. Make your changes and bump the `package.json` version.
2. Navigate to the root directory of the particular theme in a terminal. Eg - `vscode-themes/collections/lcars-theme`
3. You can test by running `npm run localinstall` and restarting VS Code.
4. When done, build: `npm run ext:package`
5. Publish the build to the VS Code marketplace: `npm run ext:publish`