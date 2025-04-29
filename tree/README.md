# fs/tree

🌳 GitHub Action that displays the tree structure of a directory and appends it to `$GITHUB_STEP_SUMMARY` as a code block.

## 📌 Features

- Uses `tree -ah` to display the directory structure.
- Formats output as a code block.
- Appends the tree structure to the GitHub step summary for easy viewing.

## 🔧 Inputs

| Name | Description                | Required | Default |
|------|----------------------------|----------|---------|
| dir  | Directory to show tree for | ✅ Yes   | `.`     |

## 🚀 Example Usage

```yaml
- name: Display project tree
  uses: actions-a3-services/fs/tree@main
  with:
    dir: ./src
```
