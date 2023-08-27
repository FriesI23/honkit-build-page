# Honkit Build Page GitHub Action

This GitHub Action automates the process of building a Honkit documentation
site from source code.

## Usage

To use this GitHub Action, follow these steps:

### 1. Add this Action to your Workflow

```yaml
- name: Build Pages
  uses: FriesI23/honkit-build-page@<version>
  with:
    nodejs-version: <overwrite node.js version>
    output-sitedir: <custom output dir>
    working-directory: <build path>
```

A specific usage example can be explored in
[.github/workflows/build-ghpage.yml](.github/workflows/build-ghpage.yml).

### 2. Enable GitHub Pages

Navigate to "`<your-repo-page>` -> `Settings` -> `Pages` -> `GitHub Pages` ->
`Build and deployment`", switch `"source"` to "GitHub Actions".

![Enbale GitHub Pages](./assets/images/enbale-github-page.png)

### 3. Commit and Push

Commit the workflow file to your repo and push it to GitHub.

## Inputs

| Input             | Description                                   |
| ----------------- | --------------------------------------------- |
| nodejs-version    | Node.js version required for building pages   |
| output-sitedir    | Final directory where the book site is stored |
| working-directory | The working directory for this action         |

See [Action](./action.yml) file to view the complete params.

## Acknowledgements

This Action was inspired by the need to simplify the process of building
Honkit documentation sites.

## License

This project is licensed under [MIT License](./LICENSE).
