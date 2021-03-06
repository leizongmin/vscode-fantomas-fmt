# fantomas-fmt README

vscode extension that uses the awesome [fantomas](https://github.com/fsprojects/fantomas) to format fsharp files.

## Requirements

- [dotnet core 2.1](https://www.microsoft.com/net/download)
- [fantomas-tool](https://github.com/fsprojects/fantomas)  
  If missing, the extension will try to install it automatically.
  In case of problem, try to install it manually by running the following command:
  ```
  dotnet tool install fantomas-tool -g
  ```

## Extension Settings

This extension contributes the following settings:

- `fantomas.indent`: set number of spaces for indentation (default = 4). The value should be between 1 and 10.
- `fantomas.pageWidth`: set the column where we break to new lines (default = 80). The value should be at least 60.
- `fantomas.preserveEOL`: preserve original end of lines, disables auto insert/remove of blank lines (default = false)
- `fantomas.semicolonEOL`: enable semicolons at the end of line (default = false).
- `fantomas.noSpaceBeforeArgument`: disable spaces before the first argument of functions when there are parenthesis (default = true).
- `fantomas.noSpaceBeforeColon`: disable spaces before colons (default = true).
- `fantomas.noSpaceAfterComma`: disable spaces after commas (default = true).
- `fantomas.noSpaceAfterSemiColon`: disable spaces after semicolons (default = true).

## Troubleshooting

1. **Format on save is not working**  
   Try to change setting "editor.formatOnSaveTimeout" to a higher value than 750 (e.g. 3000)

## License

MIT © Paolo Dellepiane
