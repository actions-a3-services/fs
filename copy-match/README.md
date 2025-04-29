# fs/copy-match

🔄 GitHub Action that copies files from a source directory to a destination directory if they match given filename prefixes.

## 📌 Features

- Takes a source and a destination directory.
- Copies files from the source to the destination if the filenames start with one of the specified prefixes.
- Supports multiple prefixes (comma-separated list).

## 🔧 Inputs

| Name   | Description                                                      | Required | Default |
|--------|------------------------------------------------------------------|----------|---------|
| source | Source directory containing files                                | ✅ Yes   | N/A     |
| dest   | Destination directory to copy matching files into                | ✅ Yes   | N/A     |
| match  | Comma-separated list of filename prefixes to match               | ✅ Yes   | N/A     |

## 🚀 Example Usage

```yaml
- name: Copy matching files
  uses: actions-a3-services/fs/copy-match@main
  with:
    source: ./build
    dest: ./dist
    match: "file1,prefix_,output"
```
