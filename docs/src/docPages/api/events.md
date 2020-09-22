# Events

:::warning Out of date
This content is written for tiptap 1 and needs an update.
:::

There are some events you can listen for. A full list of events can be found here.

```js
const editor = new Editor({
  onInit: () => {
    // editor is initialized
  },
  onUpdate: ({ html }) => {
    // get new content on update
    const newContent = html()
  },
})
```

It's also possible to register event listeners afterwards.

```js
const editor = new Editor(…)

editor.on('init', () => {
  // editor is initialized
})

editor.on('update', ({ html }) => {
  // get new content on update
  const newContent = html()
})
```