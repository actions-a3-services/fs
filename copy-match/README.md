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
| match  | List of filename prefixes to match                               | ✅ Yes   | N/A     |

## 🚀 Example Usage

```yaml
- name: Copy Matching Files
  uses: actions-a3-services/copy-matching-files@main
  with:
    source: './source_directory'
    dest: './destination_directory'
    match: |
      file1.txt
      file2.txt
      file3.txt
```
