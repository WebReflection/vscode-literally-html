# literally HTML

Adds syntax highlighting and language support for html inside of JavaScript and TypeScript tagged template strings.

Compatible with more use cases than those exposed by [vscode-lit-html](https://github.com/mjbvz/vscode-lit-html).

> **❗Important**: IntelliSense and language support requires VS Code 1.20+.

## Usage

```sh
# within your project
npm install --save-dev literally-html

# create a jsconfig.json file with the following content
echo '{
  "compilerOptions": {
    "plugins": [
      {
        "name": "typescript-lit-html-plugin"
      }
    ]
  }
}' > jsconfig.json
```
