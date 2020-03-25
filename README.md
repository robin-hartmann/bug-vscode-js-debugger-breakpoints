# 🐞 bug-vscode-node-debug2-breakpoints

Minimal working example for reproducing a bug when debugging in ts-node with Visual Studio Code

## 🛠️ Development

These instructions will get you a copy of this project up and running on your local machine for development and testing purposes.

### 📋 Prerequisites

- [Node.js](https://nodejs.org) - JavaScript run-time environment
- [Visual Studio Code](https://code.visualstudio.com/) - Code editor redefined and optimized for building and debugging modern web and cloud applications

### 🚀 Getting Started

Follow these steps to reproduce the bug:

1. Clone this project
1. Open the project's root folder in VS Code
1. Run `npm i` in the terminal to install all dependencies
1. Set a breakpoint in `src/lib.ts` on line `4`
1. Switch to the `Run` view using the side menu
1. Select the run configuration `Launch with ts-node`
1. Press `F5` to start debugging

Now the debugger should stop at the specified breakpoint, but it doesn't.

### 🚧 Workaround

1. Install the VS Code extension [JavaScript Debugger (Nightly)](https://marketplace.visualstudio.com/items?itemName=ms-vscode.js-debug-nightly) (`ms-vscode.js-debug-nightly`)
1. In `.vscode\settings.json` set `debug.node.useV3` to `true`
1. Press `F5` to start debugging

Now the debugger does in fact stop at the specified breakpoint.

## 🧰 Built With

- [TypeScript](https://www.typescriptlang.org/) - A typed superset of JavaScript that compiles to plain JavaScript
- [ts-node](https://github.com/TypeStrong/ts-node) - TypeScript execution and REPL for node.js

## 👨‍💻 Authors

- **Robin Hartmann** - [robin-hartmann](https://github.com/robin-hartmann)

## 📃 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
