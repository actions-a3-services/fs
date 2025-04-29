# fs/copy-match

📦 GitHub Action to copy files from a source directory to a destination if the filename matches specified prefixes.

## Inputs

| Name   | Description                          | Required |
|--------|--------------------------------------|----------|
| source | Directory to read files from         | ✅ Yes   |
| dest   | Directory to copy files to           | ✅ Yes   |
| match  | Comma-separated list of prefixes     | ✅ Yes   |

## Example

```yaml
- name: Copy binaries
  uses: actions-a3-services/fs/copy-match@main
  with:
    source: .opt
    dest: opt/bin
    match: psu,helper
```
