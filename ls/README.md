# fs/ls

📂 GitHub Action that lists files in a directory and appends them as a Markdown table to `$GITHUB_STEP_SUMMARY`.

## 📌 Features

- Uses `ls -la` to list files with details (permissions, owner, size, etc.).
- Formats output into a Markdown table.
- Appends the table to the GitHub step summary for visibility in Actions UI.

## 🔧 Inputs

| Name | Description            | Required | Default |
|------|------------------------|----------|---------|
| dir  | Directory to list      | ❓ No    | `.`     |

## 🚀 Example Usage

```yaml
- name: List project files
  uses: actions-a3-services/fs/ls@main
  with:
    dir: ./build
```
