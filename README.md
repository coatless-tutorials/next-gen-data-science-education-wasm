# The Next Generation of Data Science Education with WebAssembly

This repository contains the code powering **[The Next Generation of Data Science Education with WebAssembly](https://tutorials.thecoatlessprofessor.com/next-gen-data-science-education/)** Quarto website demonstration.

## Installation

To create your own version of the demonstration, you need to install the following software:

- RStudio IDE, VS Code, Positron, or another text editor
  - For VS Code or Positron, please install the [Quarto plugin](https://open-vsx.org/extension/quarto/quarto).
- [Quarto](https://quarto.org) v1.4.0 or later
- Quarto Extensions
  - [`quarto-live`](https://r-wasm.github.io/quarto-live/)
  - [`quarto-drop`](https://github.com/r-wasm/quarto-drop)
  - [`quarto-countdown`](https://github.com/gadenbuie/countdown/tree/main/quarto)
  - [`quarto-embedio`](https://github.com/coatless-quarto/embedio)

You can install the Quarto Extensions by typing the following commands in your terminal:

```bash
quarto add r-wasm/quarto-live
quarto add r-wasm/quarto-drop
quarto add gadenbuie/countdown/quarto
quarto add coatless-quarto/embedio
```

## GitHub Pages

The demonstration is hosted on GitHub Pages using a GitHub Action ([`publish-website.yml`](.github/workflows/publish-website.yml)). The action is triggered on every push to the `main` branch. The action builds the Quarto website and pushes the output to the `gh-pages`. 

Please make sure to enable GitHub Pages in the repository settings, select the GitHub Actions as the source,
and check the **Enforce HTTPS** option.

<img width="1362" alt="Setup GitHub Pages for Deploying `quarto-live`" src="https://github.com/user-attachments/assets/5c47f7a6-64ba-45f2-b3cf-2303fb801579">
