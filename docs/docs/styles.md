there is also a `style.css` file containing pre-defined css classes for `color` and `background-color`. these classes can be used in markdown files using [Attribute List](https://python-markdown.github.io/extensions/attr_list/) extension. for foreground colors, class names are `color-[color-name]` and `bg-color-[color-name]` for backgrounds:
```css
.color-red0 {
  color: var(--color-red0);
}
.bg-color-red0 {
  background-color: var(--color-red0);
}
```