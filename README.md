# Comparing Changes

A Visual Studio Code extension that highlights changes in files by marking inserted lines with `+` and deleted lines with `−`. This extension is particularly useful for comparing file changes in a structured and syntax-highlighted way.

## Features

- **Syntax Highlighting**: Provides syntax highlighting for `.cfc` files, marking inserted lines with `+` and deleted lines with `−`.
- **Custom Grammar**: Includes a TextMate grammar for `.cfc` files to tokenize and highlight changes.
- **Language Configuration**: Supports auto-closing pairs, surrounding pairs, and comment tokens for `.cfc` files.

## How to Use

1. **Install the Extension**: Click button "Install" to download

2. **Compare Files**:
   - Use the provided Python script [CompareFolder.py](https://github.com/WMZS-Modding/Tools-Scripts/blob/main/src/CompareFolder.py) to generate `.cfc` files that highlight changes between two folders.
   - Run the script with the following command:
     ```bash
     python CompareFolder.py "original_folder" -mo "modified_folder" -o "output_folder"
     ```
   - Open the generated `.cfc` files in VS Code to view the highlighted changes.

3. **Verify Syntax Highlighting**:
   - Create or open a `.cfc` file in VS Code.
   - Ensure that inserted lines are highlighted with `markup.inserted.cfc` and deleted lines with `markup.deleted.cfc`.

## Development

To modify or extend this extension:

1. Open the project in Visual Studio Code.
2. Make changes to the [cfc.tmLanguage.json](http://_vscodecontentref_/4) or [language-configuration.json](http://_vscodecontentref_/5) files as needed.
3. Reload the extension (`Ctrl+R` or `Cmd+R` on Mac) to apply changes.

## Known Issues

- The extension currently supports only `.cfc` files for highlighting changes.
- Large files may take longer to process and display.

## License

This project is licensed under the MIT License.
