# literally HTML

- - -

## WARNING

This project is inferior and not maintained as much as [htmx-literals](https://marketplace.visualstudio.com/items?itemName=lehwark.htmx-literals) is.

There is also [leet-html](https://marketplace.visualstudio.com/items?itemName=EldarGerfanov.leet-html) as alternative or [lit-html](https://marketplace.visualstudio.com/items?itemName=bierner.lit-html) so please consider using these instead as I am not planning to spend time on this any time soon.

- - -

A library agnostic fork of [vscode-lit-html](https://github.com/mjbvz/vscode-lit-html)
which aim is to bring syntax highlighting and language support for HTML inside of
any JavaScript and TypeScript tagged template strings.

> **❗Important**: IntelliSense and language support requires VS Code 1.20+.

### Example

```js
hyper(document.body)`
  <div class=${model.class}>
    ${model.greetings} !!!
  </div>`;

render`
  <ul>
    ${items.map(
      item => html`<li>${item.value}</li>`
    )}
  </ul>`;
```

## Usage

If simply installing through VS Code is not enough, maybe the following could help.

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
